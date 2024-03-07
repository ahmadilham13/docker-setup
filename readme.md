1. pastikan docker sudah terinstall di komputer
2. lakukan "docker-compose build" untuk melakukan build 
3. lakukan "docker-compose up -d" untuk melakukan build dan menjalankan container

untuk implementasi ini menggunakan port

webserver => port 1001:80
database => port 4306:3306
phpmyadmin => 1002:80

## untuk mengecek versi
1. PHP => lakukan "docker exec php_docker php --version"
2. Composer => lakukan "docker exec php_docker composer --version"
3. MySQL => lakukan "docker exec db_docker mysql --version"

## untuk mengakses mysql melalui command
1. lakukan "docker exec -it db_docker sh"
3. lakukan "mysql -u root -p"

## test crete project laravel
1. arahkan dir position to ./src
2. lakukan "docker exec php_docker composer create-project laravel/laravel ."
3. jika telah selesai instalasi laravel maka saat akses port 1001:80 akan menampilkan halaman index laravel