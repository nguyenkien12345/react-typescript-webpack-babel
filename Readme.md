Tài liệu tham khảo: https://duthanhduoc.com/blog/tao-du-an-react-webpack-typescript-babel-eslint
Khởi tạo dự án React
1) Khởi tạo một dự án nodejs
- yarn init --yes
2) Cài đặt React vào dependencies
- yarn add react react-dom
3) Cài type cho React vào devDependencies
- yarn add -D @types/react @types/react-dom typescript
4) Cài đặt Webpack
- yarn add -D webpack webpack-cli webpack-dev-server
5) Cài đặt Babel
- yarn add -D @babel/core @babel/preset-env @babel/preset-react @babel/preset-typescript babel-loader
6) Cài đặt các loader và plugins bổ trợ
- yarn add -D clean-webpack-plugin compression-webpack-plugin copy-webpack-plugin css-loader css-minimizer-webpack-plugin dotenv-webpack file-loader html-webpack-plugin mini-css-extract-plugin sass sass-loader serve webpack-bundle-analyzer
Giải thích chức năng của các plugin: 
- clean-webpack-plugin: Dọn dẹp thư mục build. Khi mà chúng ta build lần thứ 1 thì nó sẽ sinh ra những file build. Sau đó chúng ta sửa cập nhật code các kiểu chúng ta build lần thứ 2 thì nó sẽ dọn dẹp sạch sẽ cái thư mục build ở lần thứ 1 đi để nó sẵn sàng cho chúng ta 1 cái thư mục trống để chứa những cái file build mới ở lần thứ 2
- compression-webpack-plugin: Nén gzip, brotli file build
- copy-webpack-plugin: Copy các file trong thư mục public vào thư mục dist
- css-loader: import css trong dự án
- css-minimizer-webpack-plugin: minify css (minify là xóa đi những cái khoảng trống)
- dotenv-webpack: Giúp dùng được các biến môi trường trong file .env
- file-loader: import ảnh, font trong dự án
- html-webpack-plugin: Tự động thêm script và style tag vào file html
- mini-css-extract-plugin: Tách css ra thành file riêng khi build thay vì đưa vào file js
- sass: Giúp dùng sass cho dự án
- sass-loader: Cũng giúp dùng Sass cho dự án, phải cài cả 2 sass sass-loader
- serve: Giúp preview file build
- webpack-bundle-analyzer: Phân tích kích thước file build
7) Cài đặt ESLint và Prettier
yarn add -D eslint prettier @typescript-eslint/eslint-plugin @typescript-eslint/parser eslint-config-prettier eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-prettier eslint-plugin-react eslint-plugin-react-hooks eslint-webpack-plugin eslint-import-resolver-typescript

