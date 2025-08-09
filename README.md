# 📘 Keyword : `final`, `var`, and `dynamic`

In Dart (and Flutter), `final`, `var`, and `dynamic` are **keywords** used for variable declaration.  
They control how **type** and **value** behave after a variable is created.

---

## 1️⃣ `var`

- **Type is inferred** at compile time from the initial value.
- Once assigned, the **type cannot change**, but the **value can**.

### Example:
```dart
var name = "Kulani"; // Inferred as String
name = "Sharada";    // ✅ OK
// name = 10;        // ❌ Error: int can't be assigned to String

```

## 2️⃣ `final`
- Value can only be set once.
- Cannot be reassigned after being initialized.
- Type can be explicitly given or inferred.

### Example:

```dart
final city = "Colombo"; // Inferred as String
// city = "Kandy";      // ❌ Error: final variable can't be reassigned

final int age = 25;     // Explicit type
```

## 3️⃣ `dynamic`
- Type checking is disabled — can hold any type of value.
- Type can change at runtime.
- Less safe — should be used only when necessary.

### Example:
```dart
dynamic data = "Hello"; // String
data = 100;             // ✅ Now an int
data = true;            // ✅ Now a bool
```
