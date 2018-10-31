# UTS_Algoritma

## Soal 1

*Alur algoritma*

1. Deklarasikan variabel `int A, B, X, Y`
2. Masukkan input `cin >> A >> B`
3. Deklarasikan nilai `X = A; Y = B`
4. Bandingkan apakah `X != Y`
5. Bila langkah ke-4 bersifat **True** bandingkan apakah `X < Y`
6. Bila nilai `X` lebih kecil dari `Y` maka jalankan perintah `X = X+A`, bila tidak maka dijalankan perintah `Y = Y+B`
7. Cetak `cout >> X`

*Berikut code lengkapnya*
```
#include<iostream>

using namespace std;

int main() {
    int A, B, X, Y;

    cout << "Masukkan nilai A: ";
    cin >> A;

    cout << "Masukkan nilai B: ";
    cin >> B;

    X = A;
    Y = B;

    if (X!=Y) {
        if (X<Y){
            X=X+A;
        } else {
            Y=Y+B;
        }
    }

    cout << X;
}
```

## Soal 2

*Alur algoritma*

1. Deklarasikan variabel `int N, X, T, Batas`
2. Masukan input `cin >> N`
3. Deklarasikan nilai `Batas = N + 100;X = 20;T = N`
4. Selama kondisi `T <= Batas` masih bersifat **True** maka akan dikerjakan `T = T + X;X = X + 10`
5. Cetak `cout << T`

*Berikut code lengkapnya*
```
#include<iostream>

using namespace std;

int main() {
    int N, X, T, Batas;

    cout << "masukan nilai n";
    cin>> N;

    Batas = N + 100;
    X = 20;
    T = N;

    while ( T <= Batas ) {
        T= T+X;
        X=X+10;
    }

cout<< T;

}
```
