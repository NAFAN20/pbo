```dart
void main() {

  // Kelompok 1: Operator (Addition)

  int a = 10;

  int b = 5;

  print("Kelompok 1: Operator");

  print("Addition: ${a + b}");

  print("");

  

  // Kelompok 2: Map, List, Set, Symbol (List)

  List<int> numbers = [1, 2, 3, 4, 5];

  print("Kelompok 2: List");

  print("List: $numbers");

  print("");

  

  // Kelompok 3: Percabangan (If statement)

  int score = 75;

  print("Kelompok 3: Percabangan");

  if (score >= 70) {

    print("Pass");

  } else {

    print("Fail");

  }

  print("");

  

  // Kelompok 4: Perulangan (For loop)

  print("Kelompok 4: Perulangan");

  for (int i = 0; i < 5; i++) {

    print("For loop iteration: $i");

  }

  print("");

  

  // Kelompok 5: Function Parameter & Function Optional

  void greet(String name, [String? message]) {

    if (message != null) {

      print("Hello, $name! $message");

    } else {

      print("Hello, $name!");

    }

  }

  print("Kelompok 5: Function Parameter & Function Optional");

  greet("Alice");

  greet("Bob", "Welcome to Dart programming!");

  print("");

  

  // Kelompok 6: Inner Function, Function Return Value, Function Short Expression

  int add(int a, int b) {

    int sum() {

      return a + b;

    }

    return sum();

  }

  

  int multiply(int a, int b) => a * b;

  

  print("Group 6: Inner Function, Function Return Value, Function Short Expression");

  print("Addition using inner function: ${add(5, 3)}");

  print("Multiplication using short expression: ${multiply(5, 3)}");

  print("");

  

  // Group 7: Anonymous Function & Scope

  var names = ["NAFAN", "Bombong", "Hansar"];

  print("Kelompok 7: Anonymous Function & Scope");

  names.forEach((name) {

    print("Hello, $name");

  });

  

  void outerFunction() {

    var outerVar = "UTARA";

    void innerFunction() {

      var innerVar = "PRIDE!";

      print(outerVar);

      print(innerVar);

    }

    innerFunction();

    // print(innerVar);

  }

  outerFunction();

  print("");

  

  // Kelompok 8: Closure

  Function makeAdder(int addBy) {

    return (int i) => addBy + i;

  }

  print("Kelompok 8: Closure");

  var add2 = makeAdder(2);

  print(add2(3)); // 5

}
```