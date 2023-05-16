Merge Sort, diziyi böl ve fethet yaklaşımını kullanır. Bu algoritmanın aşamaları aşağıda belirtilmiştir:

**Verilen dizi:** [16,21,11,8,12,22]

 1. **Bölme aşaması:**  
    İlk olarak, verilen dizi daha küçük parçalara bölünür. 
    Bölünme işlemi, her dizi tek bir elemana indirgenene kadar tekrarlanır.  
    
   
 - [16, 21, 11, 8, 12, 22] -> [[16, 21, 11], [8, 12, 22]]  
 - [[16,21,11], [8, 12, 22]] -> [[[16], [21, 11]], [[8], [12, 22]]]  
 - [[[16], [21, 11]], [[8], [12, 22]]] -> [[[[16]], [[21], [11]]], [[[8]], [[12],[22]]]]  
 
 2. **Birleştirme aşaması:**  
        Şimdi, daha küçük parçaları karşılaştırarak ve sıralayarak büyük parçalara birleştiririz. 
        Bu işlem, tüm dizinin tamamen sıralanana kadar tekrarlanır.  

- [[[[16]], [[21], [11]]], [[[8]], [[12], [22]]]] -> [[[16], [11, 21]], [[8], [12, 22]]]  
- [[[16], [11, 21]], [[8], [12, 22]]] -> [[11, 16, 21], [8, 12, 22]]  
- [[11, 16, 21], [8, 12, 22]] -> [8, 11, 12, 16, 21, 22]  

**Sonuç:** [8, 11, 12, 16, 21, 22]  

