// go
for i := 0; i < len(x); i++ {
    v |= x[i] ^ y[i]
}

1. How are there no branches taken in the above algorithm?
