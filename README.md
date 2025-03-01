﻿# Turkish-Sign-Langauge-Recognation

 Bu Python uygulaması, Türk İşaret Dili alfabesinde bulunan rakamlar ve harfleri tanımaya yönelik bir sistem içermektedir.  Kullanılan ana kütüphaneler Mediapipe, OpenCV, Tensorflow/Keras ve diğer ilgili kütüphanelerdir.

Uygulama, Mediapipe kütüphanesi ile video akışından el hareketlerini algılamakta ve bu hareketleri görselleştirmektedir. Bu algılamalar, el landmark noktalarının 3D koordinatları ve bağlantı çizgileri ile birlikte stilize edilmiş bir şekilde görüntü üzerine çizilerek gösterilmektedir.

Eğitim verisi toplama aşamasında, belirli eylemleri gerçekleştiren kişinin el hareketlerini tanımlamak amacıyla video dizileri kullanılmaktadır. Elde edilen veriler, 3D el landmark noktalarının numpy dizileri olarak saklanmaktadır.

Model eğitimi aşamasında, LSTM ve Dense katmanları içeren bir sıralı model kullanılmakta ve bu model eğitim verisi üzerinde eğitilmektedir. TensorBoard kullanılarak eğitim süreci logları kaydedilmektedir.

Modelin performansı, test verisi üzerinde değerlendirilmekte ve çoklu etiketli karışıklık matrisi ile doğruluk oranı hesaplanmaktadır.

Son olarak, eğitilmiş model gerçek zamanlı olarak kullanılarak el hareketlerini tanımakta ve sınıflandırmaktadır. Bu gerçek zamanlı tanıma, Mediapipe ile el hareketleri tespit edilerek ve model tarafından sınıflandırılarak gerçekleştirilmektedir.

Uygulama, video akışını işleyerek kullanıcının yaptığı el hareketini gerçek zamanlı olarak tanımlayabilme yeteneği sunmaktadır.

