# Task Genius Project

Task Genius Project là một ứng dụng web quản lý task, project và user trong dự án. Ứng dụng hỗ trợ phân quyền giữa Admin và User, cung cấp các chức năng như quản lý user, theo dõi trạng thái task, và báo cáo qua biểu đồ.

## Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Environment Variables](#environment-variables)
- [Available Scripts](#available-scripts)
- [Contributing](#contributing)
- [License](#license)

## Features

- Phân quyền Admin/User.
- Quản lý user, task và project.
- Theo dõi trạng thái task bằng biểu đồ.
- Thông báo tùy chỉnh với react-hot-toast.
- Sử dụng redux-persist để lưu trữ state.
- Giao diện responsive, tích hợp Bootstrap và SCSS.

## Tech Stack

- **Frontend**: ReactJS (v18.3.1)
- **State Management**: Redux, Redux Toolkit, Redux Persist
- **Styling**: Bootstrap, SCSS
- **API Communication**: Axios
- **Charts**: Chart.js, react-chartjs-2
- **Authentication**: Firebase, JWT
- **Build Tool**: Vite

## Getting Started

### Prerequisites

Trước khi bắt đầu, bạn cần cài đặt:

- Node.js (>= 14.x)
- npm hoặc yarn

### Installation

1. Clone repository:

   ```bash
   git clone https://github.com/yenlinh139/TaskGeniusProject.git
   cd TaskGeniusProject
   ```

2. Cài đặt dependencies:

   ```bash
   npm install
   # hoặc
   yarn install
   ```

3. Tạo file `.env` dựa trên cấu hình mẫu dưới đây và điền thông tin phù hợp:

   ```env
   VITE_BASE_URL=API_BACKEND
   ```

4. Chạy dự án:
   ```bash
   npm run dev
   # hoặc
   yarn dev
   ```

Ứng dụng sẽ chạy tại: [http://localhost:5173](http://localhost:5173)

## Project Structure

```
TaskGeniusProject/
├── public/
│   └── vite.svg                 # Logo favicon
├── src/
│   ├── assets/                  # Ảnh và tài nguyên
│   ├── common/                  # Các file chung: constants, validation
│   ├── components/              # Các component tái sử dụng
│   ├── config/                  # Cấu hình axios và API
│   ├── hooks/                   # Custom hooks (usePagination)
│   ├── pages/                   # Các trang chính của ứng dụng
│   ├── store/                   # Redux store, reducers, actions
│   ├── App.jsx                  # App component chính
│   ├── main.jsx                 # Điểm vào ứng dụng
│   └── index.scss               # File SCSS chính
├── .env                         # Biến môi trường
├── index.html                   # Template HTML chính
├── package.json                 # Danh sách dependencies và scripts
└── README.md                    # Tài liệu dự án
```

## Environment Variables

Dự án sử dụng file `.env` để cấu hình biến môi trường:

```env
VITE_BASE_URL=API_BACKEND
```

Hãy thay thế `API_BACKEND` bằng giá trị thực tế từ backend của bạn.

## Available Scripts

Trong thư mục dự án, bạn có thể chạy các lệnh sau:

- **Chạy development server**:

  ```bash
  npm run dev
  ```

- **Build dự án**:

  ```bash
  npm run build
  ```

- **Preview production build**:

  ```bash
  npm run preview
  ```

- **Kiểm tra code với ESLint**:
  ```bash
  npm run lint
  ```

## Contributing

Đóng góp luôn được chào đón! Hãy làm theo các bước sau:

1. Fork dự án.
2. Tạo branch mới (`feature/your-feature-name`).
3. Commit thay đổi.
4. Tạo Pull Request.

## License

Dự án được cấp phép theo MIT License. Xem file LICENSE để biết thêm chi tiết.

