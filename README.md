### unit test
- Нийт unit test: 20 тест
- CalendarTest: 10
- OrganizationTest: 4
- PersonTest: 2
- RoomTest: 2
- MeetingTest: 2
 
Илрүүлсэн алдаа/доголдол: 2

- Calendar.addMeeting containment overlap илрүүлэхгүй: 10–12 байгаа үед 9–13-ыг зөвшөөрөх ёсгүй. Үүнийг барих testContainmentOverlap_expectedToFailCurrentLogic тест нэмсэн бөгөөд одоогийн хэрэгжилт дээр тэр тест алдаж (intended fail) байна.
- Calendar.checkTimes сард 12-ыг буруу няцаадаг: mMonth >= 12 гэсэн шалгалтаас шалтгаалж 12-р сар буруугаар “Month does not exist.” алдаа өгдөг логик доголдол байна (кодын үзлэгээр тогтоосон). Үүнийг засахдаа mMonth > 12 болгох шаардлагатай.
  
### Хамрах хүрээ
- Зөв кейсүүд: Энгийн уулзалт, бүтэн өдрийн амралт/блок, өрөө/хүн завгүй эсэх, agenda хэвлэх, байгууллагын обьект хайлт.
- Алдаат кейсүүд: Буруу сар/өдөр/цаг, start >= end, өрөө/хүн олдохгүй, өргөн хүрээтэй давхцал.
