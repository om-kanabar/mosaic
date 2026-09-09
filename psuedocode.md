function plausability(z):
    return plaus_score

function updateLists(D,U, i):
    if !D or/and U
        return
    elif i:
        U.add(i)
    P = D-U
    return P


function select_samples(P):
    i = random sample from P
    updateLists(D, U, i)
    j = random sample from P
    updateLists(D, U, j)
    return [i,j]

function 