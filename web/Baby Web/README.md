**Baby Web**

Тайлбар 
    
    http://218.100.84.112:9004

 
Энэ даалгавар дээр hint өгөгдсөнөөр бид source -г харах боломжтой болсон юм. 

Source code -г  Logmein3 даалгавартай ижил == operator ашигласныг харж болно. Гараас оруулсан тэмдэгтийн урт нь 4 өөс бага байх ёстой боловч утга нь 999 ээс их байх ёстой гэнэ.

[![N|Solid](https://github.com/DCERT-MNDC/HZ-U18-2018/blob/master/include/baby.png)](https://github.com/DCERT-MNDC/HZ-U18-2018/blob/master/include/baby.png)

999 – 1000 -ийн хооронд энэ нөхцлийг хангах тоо байхгүй. Харин == алдааг ашиглан.

    var_dump(4 > strlen("3e6")); // 4 >  3 -> true

    var_dump(999 > "3e6"); // 999 >  3e6 (3e6 = 3x10^6 = 3000000) -> true


3e3- > 3e9 ийн хооронд аль ч утгыг оруулсан шалгалтыг давж чадаж байна. 

[![N|Solid](https://github.com/DCERT-MNDC/HZ-U18-2018/blob/master/include/baby2.png)](https://github.com/DCERT-MNDC/HZ-U18-2018/blob/master/include/baby2.png)

Бид Logmein3 болон Baby web 2оос юу сурав гэхээр хэрвээ php дээр 2 хувьсагч жиших гэж байгаа бол ===  ашиглах хэрэгтэй 😉
