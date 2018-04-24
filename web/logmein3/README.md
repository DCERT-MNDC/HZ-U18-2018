Logmein3 

Тайлбар 

http://218.100.84.112:9001 

Өгөгдсөн линк-ийн дагуу орж харвал энгийн login form угтлаа.  Сонирхолтой нь тус form ийн source өгөгдсөн байв. Ажиглавал гараас оруулсан өгөгдөл нь өөр хоорондоо ялгаатай байхыг шаардах бөгөөд харин тэдний md5 хэш нь ижил байх ёстой гэнэ. Ийм байх боломжтой гэж үү? 
 
[![N|Solid](https://github.com/DCERT-MNDC/HZ-U18-2018/blob/master/include/log3.png)](https://github.com/DCERT-MNDC/HZ-U18-2018/blob/master/include/log3.png)

Сайн ажиглавал энд md5($_POST['username'])==md5($_POST['password']) байх ба  php дээр ==   хэрвээ тэмдэгтийг  тоотой харьцуулбал тэмдэгтийг хүчээр тоо руу хөрвүүлж харьцуулдаг байдаг. Жишээ нь : 

var_dump(0 == "a"); // 0 == 0 -> true

var_dump("1" == "01"); // 1 == 1 -> true

var_dump("10" == "1e1"); // 10 == 10 -> true

var_dump(100 == "1e2"); // 100 == 100 -> true

энийг ашиглан хэрвээ md5 хэш нь 0e* ээр эхэлсэн тэмдэгтүүдийг олж чадвал бид энэ шалгалтыг давах боломжтой болж байгаа юм. 

Хэсэг google хайлт хийснээр үүнийг давах  утгуудыг олж чадлаа. 
   
     $ echo -n 240610708 | md5sum
      0e462097431906509019562988736854  - 
      $ echo -n QNKCDZO | md5sum
      0e830400451993494058024219903391  -
      $ echo -n aabg7XSs | md5sum
      0e087386482136013740957780965295  -

Эндээс аль нэг 2 утгыг оруулснаар flag -г гаргаж авав. 

[![N|Solid](https://github.com/DCERT-MNDC/HZ-U18-2018/blob/master/include/log3-2.png)](https://github.com/DCERT-MNDC/HZ-U18-2018/blob/master/include/log3-2.png)
