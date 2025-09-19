# AHDM
BaiTap_AHDM
"""
Demo GitHub Branch với 1 file Python duy nhất
- Chứa lời chào
- Các phép toán cơ bản
- Một menu CLI đơn giản
"""

def say_hello(name):
    """
    Trả về lời chào kèm tên người dùng.
    """
    return f"Xin chào, {name}!"


def add(a, b):
    return a + b


def subtract(a, b):
    return a - b


def multiply(a, b):
    return a * b


def divide(a, b):
    if b == 0:
        raise ValueError("Không thể chia cho 0")
    return a / b


def menu():
    print("=" * 40)
    print("CHƯƠNG TRÌNH DEMO GITHUB BRANCH")
    print("=" * 40)
    print("1. Lời chào")
    print("2. Cộng hai số")
    print("3. Trừ hai số")
    print("4. Nhân hai số")
    print("5. Chia hai số")
    print("0. Thoát")
    print("=" * 40)


def main():
    while True:
        menu()
        choice = input("Chọn chức năng: ")

        if choice == "1":
            name = input("Nhập tên: ")
            print(say_hello(name))

        elif choice == "2":
            a = int(input("Nhập số a: "))
            b = int(input("Nhập số b: "))
            print("Kết quả:", add(a, b))

        elif choice == "3":
            a = int(input("Nhập số a: "))
            b = int(input("Nhập số b: "))
            print("Kết quả:", subtract(a, b))

        elif choice == "4":
            a = int(input("Nhập số a: "))
            b = int(input("Nhập số b: "))
            print("Kết quả:", multiply(a, b))

        elif choice == "5":
            a = int(input("Nhập số a: "))
            b = int(input("Nhập số b: "))
            try:
                print("Kết quả:", divide(a, b))
            except ValueError as e:
                print("Lỗi:", e)

        elif choice == "0":
            print
