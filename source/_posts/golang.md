---
title : Pengalaman Belajar Bahasa Go lang
---

> ***Halloo people, kali ini frda akan membagikan 
pengalaman bagaimana mengenal belajar bahasa  baru yang lagi booming ***

![](https://cdn-images-1.medium.com/max/1600/0*fyyS1OHEaQ2il8Tg.png)


Sebelumnya pernah denger ada bahasa baru yang cukup booming, frda bertanya-tanya mengenai bahasa baru ini, temen-temen yang belum tau  bahasa Go lang itu apa, mungkin pertanyaannya bakalan sama kayak frda.


#### 1. Apasih Go/Go lang itu?

Awalnya frda beranggapan kalo `Go` itu adalah bahasanya dan `Go lang` adalah frameworknya, jadi kayak berpasangan gitu. Tapi itu salah total bung hehehe. 
Sebenernya bahasa `Go` dan `Go lang` itu sama aja. nama asli bahasanya adalah `GO`, tapi karena terlalu umum jadi ditambahin `lang` dibelakangnya sehingga sekarang terkenal dengan nama `Go lang/Golang`.

#### 2. Kenapa Se-booming ini di kalangan programmer?

Frda bilang se-booming ini karena setiap ada event mengenai programming selalu ada sentilan bahasa Go, orang - orang ngomongin bahasa Go ini. 
Ternyata faktanya adalah :

* Bahasa Go adalah bahasa yang paling cepat eksekusinya dibandingkan dengan c#, javascript,dotNet dan lain -lainnya. `Go lang` ini eksekusinya/compilenya diibaratkan langsung ngomong ke komputer ga lewat interface. Hal ini bisa dibuktikan dan di tes dengan namanya benchmark, yang frda ketahui benchmark itu fitur di visual studio code yang berbentuk fungsi untuk membandingkan kecepatan eksekusi beberapa bahasa. Syntaxnya seperti ini `go test -bench`

* Error Checking nya mantap, bisa dibilang `Go lang` ini pemberitahu yang baik, selalu ngingetin kalo ada  variabel yang gak kepake(UnUsed) dia langsung error.

* Cross Compiling, Go lang itu executable nya file binary

* Garbage Collection, Go lang bakal me-manage memorinya secara otomatis

* Scalability nya mendukung microservices dan modular

* Simplicity katanya simpel

* Syntaxnya agak berbeda dari yang lain, contohnya for each dalam Go:

```
    for index, element := range someSlice {
        // index is the index where we are
        // element is the element from someSlice for where we are
    }
    If you don't care about the index, you can use _:

    for _, element := range someSlice {
        // element is the element from someSlice for where we are
    }
```    

* Bahasa Go ini lebih cocok dengan framework `Echo` karena kecepatan eksekusinya. Framework `Echo` sendiri merupakan framework Go yang High performance, extensible, dan minimalist.

![](https://echo.labstack.com/images/terminal.png)


#### 3. Bagaimana Testing dalam Go?

Sebenernya ini pertanyaan yang belum kesampaian tapi tutorku memeperkenalkannya. Dalam Golang ada namanya TEST DRIVEN DEVELOPMENT atau disingkat TDD.
TDD adalah kita membuat test nya dulu untuk fungsi apa saja yang nanti akan digunakan, baru bikin kodingannya, atau bisa berbarengan satu - satu program/kodingan di buat lalu bikin test nya. Sehingga nanti kalo kodingannya banyak dan mau nambah fitur dalam aplikasi kita kita bisa tau dengan mudah errornya dimana dan lebih baik menambah fitur dimana.  

![](https://cdn-images-1.medium.com/max/1600/1*Mjb3IFooRmFumA2IgNEWbw.png)






