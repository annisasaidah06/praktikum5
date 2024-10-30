# praktikum5
# Profil

| Variable | Isi |
| -------- | --- |
|**Nama**  | Annisa Saidah Mubarokah |
|**NIM**   | 312310631 |
|**Kelas** | TI.23.A6 |
|**Mata Kuliah** | pemograman beriotensi objek |

# Praktikum5

## Class Utama

```java
package praktikum.pkg5;

public class Utama {

    public static void main(String[] args) {
        Lingkaran lingkaran = new Lingkaran(5);
        System.out.println("Luas Lingkaran: " + lingkaran.luas());
        System.out.println("Keliling Lingkaran: " + lingkaran.keliling());

        Segitiga segitiga = new Segitiga(4, 6);
        System.out.println("Luas Segitiga: " + segitiga.luas());

        Persegi persegi = new Persegi(7);
        System.out.println("Luas Persegi: " + persegi.luas());
        System.out.println("Ke leling Persegi: " + persegi.keliling());
    }
}
```
![](ss/Class%20Utama.jpeg)

## Bangun Datar

```java
package praktikum.pkg5;

class BangunDatar {
    public float luas() {
        return 0;
    }
    
    public float keliling() {
        return 0;
    }
}
```


## Lingkaran

```java
package praktikum.pkg5;

class Lingkaran extends BangunDatar {
    private final int r;
    
    public Lingkaran(int r) {
        this.r = r;
    }

    @Override
    public float luas() {
        return (float) (Math.PI * r * r);
    }

    @Override
    public float keliling() {
        return (float) (2 * Math.PI * r);
    }
}
```

![](ss/Lingkaran.jpeg)


## Persegi

```java
package praktikum.pkg5;

class Persegi extends BangunDatar {
    private final int sisi;
    
    public Persegi(int sisi) {
        this.sisi = sisi;
    }

    @Override
    public float luas() {
        return (float) (sisi * sisi);
    }

    @Override
    public float keliling() {
        return (float) (4 * sisi);
    }
}
```

![](![Persegi](https://github.com/user-attachments/assets/6ecaef41-c9d1-450e-aeae-6aef98913b57)
)

## Segitiga

```java
package praktikum.pkg5;

class Segitiga extends BangunDatar {
    private final int alas;
    private final int tinggi;
    
    public Segitiga(int alas, int tinggi) {
        this.alas = alas;
        this.tinggi = tinggi;
    }

    @Override
    public float luas() {
        return (float) (0.5 * alas * tinggi);
    }

    @Override
    public float keliling() {
        return (float) (alas + alas + tinggi);
    }
}
```

![](![Segitiga](https://github.com/user-attachments/assets/e447aeaf-e3df-4704-97a1-faa4f3f558e1)
)

## Output

![Output](https://github.com/user-attachments/assets/6432fe7a-3fc0-4cf3-8456-3fe7336fa657)

