# two_sum-pratise
tập bài tập leet code - bài 1: 2 tổng
# Cho một mảng các số nguyên nums và một số nguyên target, 
# hãy trả về các chỉ số của hai số trong mảng sao cho tổng của chúng bằng target.
def two_sum( number, target): 
    for i in range(len(number)): 
        for j in range( i + 1, len(number)):
            if number[i] + number[j] == target: 
                return [i,j]
            
number = [2, 7, 11, 15]
target = 13
print (two_sum(number, target))
# Dòng 3: khai báo số và mảng
# Dòng 4: duyệt qua các mục trong mảng numbers
#       range(len(number)): tạo ra 1 dãy số từ 0 đến len(number) - 1
#        i là chỉ số phần tử hiện tại trong vòng lặp
# Dòng 5: Vòng lặp này bắt đầu từ chỉ số i + 1 và tiếp tục đến cuối mảng.
#       j là chỉ số của phần tử tiếp theo mà chúng ta sẽ kiểm tra tổng với phần tử i.
# Dòng 6: kiểm ra xem tổng của number[i] + number[j] có = target hay không
# VD: Cho mảng nums = [2, 7, 11, 15] và target = 9:
#       Vòng lặp đầu tiên: i = 0, tức là nums[0] = 2.
#       Vòng lặp bên trong: j = 1, tức là nums[1] = 7.
#       Ta kiểm tra tổng: 2 + 7 = 9, đúng bằng target, nên hàm trả về [0, 1]
