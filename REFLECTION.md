# REFLECTION

## 1. Хамгийн үнэ цэнэтэй assertion
Status code болон business rule assertion хамгийн хэрэгтэй санагдсан. Учир нь API зөвхөн 200 буцаах биш бодит өгөгдөл зөв эсэхийг шалгах шаардлагатай байдаг.

## 2. Negative test
GET /users/999999 endpoint дээр 404 status шалгасан. Энэ тест нь backend байхгүй хэрэглэгч дээр зөв алдаа буцааж байгаа эсэхийг баталгаажуулдаг.

## 3. Newman дээр fail болсон эсэх
Эхэндээ environment variable дутуу байсан тул Newman дээр fail болсон. Postman дотор local variable байсан учраас ажиллаж байсан.

## 4. Secret management
Token болон secret-уудыг env.dev.json дээр placeholder хэлбэрээр хадгалсан. GitHub дээр жинхэнэ token commit хийгээгүй.

## 5. Эмзэг хэсэг
Response schema өөрчлөгдвөл тестүүд хамгийн их эвдэрнэ. Үүнийг багасгахын тулд schema validation-ийг flexible байдлаар бичих хэрэгтэй.
