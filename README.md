# HC-SR04-Ultrasonic-Sensor
HC-SR04 Ultrasonic Sensor ile mesafe ölçümü

![HCSR04 Ultrasonic Sensor çalışması](https://github.com/zyakkoc/HC-SR04-Ultrasonic-Sensor/blob/main/HCSR04.jpg)

Zamanlama diyagramı aşağıda gösterilmiştir. Mesafeyi başlatmak için tetik girişine yalnızca kısa bir 10uS darbesi sağlamanız gerekir ve ardından modül 40 kHz'de
8 döngülü bir ultrason patlaması gönderir ve yankısını yükseltir. Yankı, darbe genişliği ve menzili orantılı olan bir mesafe nesnesidir. Tetik sinyali gönderme 
ve yankı sinyali alma arasındaki zaman aralığı boyunca aralığı hesaplayabilirsiniz. Formül: uS / 58 = santimetre veya uS / 148 = inç; veya: aralık = yüksek 
seviye zaman * hız (340M/S) / 2; yankı sinyaline tetikleme sinyali gelmesini önlemek için 60 ms'den fazla ölçüm döngüsü kullanmanızı öneririz.

dwt_stm32_delay.c ve dwt_stm32_delay.h dosyaları mikrosaniye için hazır kütüphanelerdir.
