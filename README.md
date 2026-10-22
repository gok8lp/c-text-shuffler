# C Text Shuffler

Girilen metnin karakterlerinin sırasını rastgele değiştiren küçük C alıştırması.
A C learning exercise that shuffles the characters of an input word.

Bu program yeni ve bağımsız karakterlerden parola üretmez; kullanıcıdan aldığı karakterleri farklı sıraya koyar.
Bu yüzden depo adı yaptığı işi anlatacak şekilde düzenlenmiştir.

## Derleme ve kullanım

```bash
gcc -std=c11 -Wall -Wextra shuffle_text.c -o shuffle_text
./shuffle_text
```

Bir kelime girilir; program rastgele indeks sırasıyla aynı karakterleri yeniden yazar.
Karakterler girişte tekrar ediyorsa çıktıda da tekrar edebilir.

## Öğrenme konusu ve sınırlar

Dizi, string uzunluğu, rastgele indeks ve kullanılan indeksleri kontrol etme.
Kod bir ilk denemedir: mevcut `scanf("%s", ...)` uzun girdiyi sınırlamaz; bellek taşması riski vardır.
`rand()` kriptografik rastgelelik sağlamaz. Gerçek parola üretimi için kullanılmamalıdır.
