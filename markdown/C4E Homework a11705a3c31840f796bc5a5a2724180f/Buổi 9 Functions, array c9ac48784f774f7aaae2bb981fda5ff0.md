# Buổi 9: Functions, array

1. Tạo một function chuyển đổi nhiệt độ nhận vào hai parameter
    
    Param 1 là “value” là cái giá trị number của nhiệt độ đó
    
    Param 2 là “mode” có thể là “c2f” hoặc “f2c” (celsius và fahrenheit), nếu không phải là một trong hai cái kia thì return lại ngay giá trị của param 1
    
    ⇒ Trả về giá trị đã quy đổi nhiệt độ, tự google công thức toán đổi giữa C ⇒ F và F ⇒ C
    
2. Viết một hàm nhận vào một mảng bất kì
    1. Nếu hàm đó có bất kì phần tử nào không phải số thì return lại mảng ban đầu
    2. Nếu các phần tử đều là số thì trả về mảng đó sắp xếp từ nhỏ đến lớn (tham khảo hàm .sort() của array trên google)
    
    VD: input: [4, 3, 25, 10] ⇒ Output: [3, 4, 10, 25]
    
    input: [”hello”, 3, 5] ⇒ Output: [”hello”, 3, 5]