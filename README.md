# Types of Function in Dart
Funtion คือ block ของ code ที่จะรันเมื่อถูกเรียก เราสามารถใส่ data ที่เรียกว่า parameters เข้าไปในฟังก์ชั่นได้ โดยฟังก์ชั่นจะคืนค่า (return) เป็นผลลัพธ์

## ประเภทของ Function มีดังนี้
  1. No Parameter And No Return Type
  2. Parameter And No Return Type
  3. No Parameter And Return Type
  4. Parameter And Return Type


## Function With No Parameter And No Return Type

  ฟังก์ชันนี้ไม่ต้องส่งพารามิเตอร์และ ไม่มีการคืนค่าจากฟังก์ชัน

### Example:

	void main() {
	  printName();
	}
	void printName() {
	  print("My name is John Doe.");
	}

### Output: 
	---> My name is John Doe.

ตามตัวอย่าง printName() คือฟังก์ชันที่มีคีย์เวิร์ด void หมายความว่าไม่มีประเภทการส่งคืน และวงเล็บว่างแสดงว่าไม่มีพารามิเตอร์ที่ส่งผ่านไปยังฟังก์ชัน

## Function With Parameter And No Return Type

  ฟังก์ชันนี้ต้องส่งพารามิเตอร์และ ไม่มีการคืนค่าจากฟังก์ชัน
	
### Example:

	void add(int a, int b) {
	  int sum = a + b;
	  print("The sum is $sum");
	}
	void main() {
      int num1 = 10;
	  int num2 = 20;
	  add(num1, num2);
	}

### Output: 
	---> The sum is 30

ตามตัวอย่าง add(int a, int b) คือฟังก์ชันที่มีคีย์เวิร์ด void หมายความว่าไม่มีประเภทการส่งคืน และวงเล็บไม่ว่าง แสดงว่ามีการส่งค่าพารามิเตอร์ไปยังฟังก์ชัน จากตัวอย่างส่งพารามิเตอร์ประเภท int

## Function With No Parameter And Return Type

  ฟังก์ชันี้ไม่ต้องส่งพารามิเตอร์และมีการคืนค่าจากฟังก์ชัน
	
### Example:

	void main() {
	  String name = primeMinisterName();
	  print("The Name from function is $name.");
	}
	String primeMinisterName() {
 	  return "John Doe";
	}

### Output:  
	---> The name from function is John Doe

ตามตัวอย่าง primeMinisterName() คือฟังก์ชันที่มีคีย์เวิร์ด String นำหน้าชื่อฟังก์ชัน หมายความว่าจะส่งกลับค่า String และวงเล็บว่างแสดงว่าไม่มีพารามิเตอร์ที่ถูกส่งผ่านไปยังฟังก์ชัน

## Function With Parameter And Return Type

  ฟังก์ที่ต้องส่งพารามิเตอร์และมีการคืนค่าจากฟังก์ชัน
	
### Example:

	double calculateInterest(double principal, double rate, double time) {
	  double interest = principal * rate * time / 100;
	  return interest;
	}
	void main() {
	  double principal = 5000;
	  double time = 3;
      double rate = 3;
      double result = calculateInterest(principal, rate, time);
      print("The simple interest is $result.");
	}

### Output: 
	---> The simple interest is 450.0.

ตามตัวอย่าง calculateInterest(double principal, double rate, double time) คือฟังก์ชันที่มีคีย์เวิร์ด double นำหน้าชื่อฟังก์ชัน หมายความว่าจะส่งกลับค่า double และวงเล็บไม่ว่าง แสดงว่ามีการส่งค่าพารามิเตอร์ไปยังฟังก์ชัน จากตัวอย่างส่งพารามิเตอร์ประเภท double
