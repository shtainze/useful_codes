# Source:
# https://note.nkmk.me/en/python-list-flatten/#flatten-3d-or-higher-dimensional-lists-and-lists-with-non-iterable-elements

def flatten_single(l):
    for el in l:
        if isinstance(el, collections.abc.Iterable) and not isinstance(el, (str, bytes)):
            yield from flatten(el)
        else:
            yield el


def flatten(l):
    return list(flatten_single(l))
