# lotri matrix parsing

    $id
        et1
    et1   1
    
    $id2
        et2
    et2   3
    
    Properties: df 

---

    List of 3
     $ id : num [1, 1] 1
      ..- attr(*, "dimnames")=List of 2
      .. ..$ : chr "et1"
      .. ..$ : chr "et1"
     $ id2: num [1, 1] 3
      ..- attr(*, "dimnames")=List of 2
      .. ..$ : chr "et2"
      .. ..$ : chr "et2"
     $ df :List of 1
      ..$ id: num 3

# fixed tests

         a    b    c
    a 40.0  0.1  0.1
    b  0.1 20.0  0.1
    c  0.1  0.1 30.0
    this matrix has fixed elements

# Combined estimates and matrix

    Lotri Estimates (get with `lotriEst()`):
      name lower est upper   fix   label backTransform
    1    a     0   1   Inf FALSE a label           exp
    2    b     0   1     2 FALSE    <NA>          <NA>
    3    c  -Inf   1   Inf  TRUE    <NA>          <NA>
    4    d     0   1     2  TRUE    <NA>          <NA>
    5    e     0   1     2  TRUE    <NA>          <NA>

---

    Lotri Estimates (get with `lotriEst()`):
      name lower est upper   fix   label backTransform
    1    a     0   1   Inf FALSE a label           exp
    2    b     0   1     2 FALSE    <NA>          <NA>
    3    c  -Inf   1   Inf  TRUE    <NA>          <NA>
    4    d     0   1     2  TRUE    <NA>          <NA>
    5    e     0   1     2  TRUE    <NA>          <NA>
    
    Matrix:
        f   g
    f 1.0 0.5
    g 0.5 1.0

# as.data.frame

    Lotri Estimates (get with `lotriEst()`):
      name lower est upper   fix   label backTransform
    1    a     0   1   Inf FALSE a label           exp
    2    b     0   1     2 FALSE    <NA>          <NA>
    3    c  -Inf   1   Inf  TRUE    <NA>          <NA>
    4    d     0   1     2  TRUE    <NA>          <NA>
    5    e     0   1     2  TRUE    <NA>          <NA>
    
    Matrix:
        f   g
    f 1.0 0.5
    g 0.5 1.0
    this matrix has fixed elements

---

    Lotri Estimates (get with `lotriEst()`):
       name lower est upper   fix   label backTransform
    1     a     0   1   Inf FALSE a label           exp
    2     b     0   1     2 FALSE    <NA>          <NA>
    3     c  -Inf   1   Inf  TRUE    <NA>          <NA>
    4     d     0   1     2  TRUE    <NA>          <NA>
    5     e     0   1     2  TRUE    <NA>          <NA>
    6     h     0   1   Inf FALSE b label         expit
    7     i     0   1     2 FALSE    <NA>          <NA>
    8     j  -Inf   1   Inf  TRUE    <NA>          <NA>
    9     k     0   1     2  TRUE    <NA>          <NA>
    10    l     0   1     2  TRUE    <NA>          <NA>
    
    $id
        m   n
    m 1.0 0.5
    n 0.5 1.0
    
    $occ
        f   g
    f 1.0 0.5
    g 0.5 1.0
    this matrix has fixed elements
    

