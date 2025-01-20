# patikaodev
### **Insertion Sort Aşamaları**

Verilen dizi: **[22, 27, 16, 2, 18, 6]**

**1. Adım:**
Başlangıçta dizi: **[22, 27, 16, 2, 18, 6]**  
İlk sayı olan 22'yi sıralı alt dizi olarak kabul ediyoruz.  
Bundan sonraki öğeleri tek tek karşılaştıracağız ve uygun yerlerine yerleştireceğiz.

**2. Adım:**
İkinci sayı olan 27'yi, sıralı alt dizi olan [22] ile karşılaştırıyoruz.  
27, 22'den büyük olduğu için sıralı dizide kalır.  
Dizi: **[22, 27, 16, 2, 18, 6]**

**3. Adım:**
Üçüncü sayı olan 16'yı, sıralı dizi [22, 27] ile karşılaştırıyoruz.  
16, 27'den küçük olduğu için 27'nin önüne geliyor.  
Daha sonra 16, 22'den de küçük olduğu için 22'nin önüne geliyor.  
Dizi: **[16, 22, 27, 2, 18, 6]**

**4. Adım:**
Dördüncü sayı olan 2, sıralı dizi [16, 22, 27] ile karşılaştırıyoruz.  
2,16'dan daha küçük olduğu için dizinin en başına yerleştiriyoruz.  
Dizi: [2, 16, 22, 27, 18, 6]

**5. Adım:**
Beşinci sayı olan 18'i, alt dizi [2, 16, 22, 27] ile karşılaştırıyoruz.  
18, 27'den küçük ancak 22'den büyük olduğu için 22 ile 27 arasına yerleşir.  
Dizi: **[2, 16, 18, 22, 27, 6]**

**6. Adım:**
Son sayı olan 6, sıralı alt dizi [2, 16, 18, 22, 27] ile karşılaştırılır.  
2'den büyük ve diğer tüm sayılardan küçük olduğu için 2'nin sonrasına yerleşir.  
Dizi: **[2, 6, 16, 18, 22, 27]**

**Sonuçta sıralı dizi:** **[2, 6, 16, 18, 22, 27]**

----------

### **Big-O Gösterimi**

- **Best Case (En İyi Durum):** O(n)  
  Eğer dizi zaten sıralıysa, her sayı sadece bir kez karşılaştırılır ve sıralama işlemi çok hızlı gerçekleşir.

- **Worst Case (En Kötü Durum):** O(n²)  
  Eğer dizi tam ters sırada ise, her öğe için sıralı alt dizinin başından sonuna kadar karşılaştırma yapılır. Bu da O(n²) karmaşıklığına yol açar.

- **Average Case (Ortalama Durum):** O(n²)  
  Ortalama durumda, her öğe sıralı alt dizi ile kısmi karşılaştırmalar yapar ve genellikle bu işlem O(n²) zaman alır.

----------

### **Time Complexity**

**Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer?**

18 sayısı [2, 6, 16, 18, 22, 27] sıralı dizisinde **ortalama durumu** ifade eden **"Average Case"** durumuna girer.

**Sebep:**  
- 18 sayısı dizide ortada bir yerde bulunuyor ve alt dizinin bir parçası olarak konumlandırılmış. Ortalama durumda aradığınız sayılar sıralı dizide ortada veya sonunda yer alabilir.
-----------

### **Selection Sort**

**Dizi** [7, 3, 5, 8, 2, 9, 4, 15, 6]
**1. Adım** [2, 3, 5, 8, 7, 9, 4, 15, 6]
**2. Adım** [2, 3, 4, 8, 7, 9, 5, 15, 6]
**3. Adım** [2, 3, 4, 5, 7, 9, 8, 15, 6]
**4. Adım** [2, 3, 4, 5, 6, 9, 8, 15, 7]
