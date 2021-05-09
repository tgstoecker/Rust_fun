A basic hello world in Rust:
```
fn main() {
    println!("Hello, Tyll! I love Rust :D"); 
}
```

About the primitives/ basic types in Rust:
```
    let x = 1;
    // x = 2;
    // this would not work since in Rust by default variables are immutable

    // we can however specify and get a mutable variable using the "mut" flag
    let mut y = 3;
    y = 4;

    // Rust tries to infer the type of the variable however we can be orderly & specific
    let z: u32 = 5;
   
    // This leads to the Primitives/ basic types that we have in Rust:
    // for integers:
    // i8, u8, i16, u16, i32, u32, i64, u64
    // also sizes numbers - memory size will differ based on the system architecture you are on
    // 64bit machine, then this will default to 64 bits 
    // isize, usize
    // we also have to float types
    // f32 (single precision); f64 (double precision)

    // we can also perform basic math in Rust
    let a = 1 + 2;
    let b = 5 - 4;
    let c = 2 * 3;
    let d = 4 / 2;
    // modulo
    let e = 26 % 8;

    // also bool types
    // bool: true/false

    // character types
    // important! - they are denoted by SINGLE quotes '' unlike str type with ""
    //let f = 'f';
    let f: char = 'f';
    // ASCII based, so everything goes here: Emojis, asian characters etc.alloc

    // we also have tuples in Rust
    // don't have to be same type!
    let g: (i32, f64, char) = (84, 6.77, 'S');
    // tuples are useful for quite a lot of things; e.g. destuctering
    // e.g.
    //let g2: (h, i, j) = g;
    // pattern matching will be performed and h will be assigned to i32; i to h64 and so on..
    // but we can also leave some out and only assigned to be char
    //let g3: (_, _, j) = g;
    // tuples can accessed via index calls, e.g
    // g.0 = 84

    // lastly arrays - basically lists of ONE type
    let k = [1,2,3,4,5,6,7,8,9];
    let k2 = k[0]; // will give us 1

    // BOTH tuples and Arrays are ZERO indexed
    // arrays can't change their size even when they are mutable
    // not very flexible - but there other datatypes like vectors which can change their size and much more
```