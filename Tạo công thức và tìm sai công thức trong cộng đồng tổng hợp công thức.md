# tạo vòng lặp While
while True:
# huớng dẫn
	print(' chọn công thức')
	print('nhập 1 để chọn công thức tổng quát của cấp số cộng \n nhập 2 để chọn tìm công sai d trong công thức tổng quát')

# biến nhập lựa chọn và để chạy if
	lua_chon = int(input('nhập lựa chọn của bạn:'))
#nhập 1 sẽ dẫn thẳng tới công thức tổng quát tìm Un
	if lua_chon == 1:
		print('công thức tổng quát củacấp số cộng')

# công thức
		print(' Un = U1+(n-1)d')
# nhập số cần tính
		U1 = int(input(' số hạng đầu U1: '))
		n = int(input(' số hạng cần tìm Un: '))
		d = int(input('công sai d'))
#kt n - 1 khác 0
		if n - 1 !=0:
#in ra công thức nhưng không cho ra kết quả
			print(' ta có công thức:', U1,' + , (',n,' - 1) × ',d)
#kết quả
			print('Kết quả của bạn là:', U1 + (n-1)*d)
			
		else:
			print('số không hợp lệ vui lòng nhật số khác')
# khi nhập 2 sẽ rẽ bạn qua tìm công sai d
	elif lua_chon == 2:
		print('tổng quát tìm công sai d')
#công thức
		print('[d = Un - U1/n - 1')
#nhập số cần tính
		U1 = int(input(' số hạng đầu U1: '))
		Un = int(input('số hạng Un'))
		n = Un
		d = 'd'
#kt giá trị n - 1 khác 0
		if n - 1 != 0:
#in ra công thức nhưng không cho ra kết quả
			print('ta có', d, '=', Un, '-', U1,' / ', n , '-1')
			print('kết quả của bạn là:',(Un - U1) / (n-1))
			
		else:
			print('số không hợp lệ vui lòng nhật số khác')
#khi nhập số khác 1 và 2 sẽ báo không hợp lệ
	else:
		print('lựa chọn không hợp lệ')
#khi lựa chọn không hợp lệ sẽ nhập lại
	tiep_tuc = input('Bạn có muốn tiếp tục không? (nhập "yes" để tiếp tục): ')
	if tiep_tuc.lower() != 'yes':
		break
		
