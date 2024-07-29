# Full-Stack Drug Search & Tracker Application

## 📚 Table of Contents

- [Postman Collection](#postman-collection)
- [Demo Video](#demo-video)
- [Setup and Installation](#setup-and-installation)
- [About](#about)


## Postman Collection
The api endpoints are neatly organized and carefully documented in this postman collection: https://documenter.getpostman.com/view/14910036/2sA3kaCKEF

## Demo Video

https://youtu.be/skOtX5z-Dts

## Setup and Installation

### Clone this repository

```bash
git clone https://github.com/mhasan341/HCTakeHomeChallenge.git
cd HCTakeHomeChallenge
git submodule update --init --recursive
```
### Now we have two repositories

```bash
cd Laravel
cp .env.example .env
composer install
```
Edit the .env and add a database

### Seeding is important as it creates some permissions and other data to be used.
```bash
php artisan migrate --seed

php artisan key:generate

php artisan serve
```

(optional)
For any permission related issue, please provide permission to the following folder.

```bash
chmod -R 775 storage
chmod -R 775 bootstrap/cache
```

# About

### Laravel Backend

- **User Authentication**: Secured by Sanctum
- **Drug Search** (Public)
- **User Medications** (Private & all essential api)
- **Error Handling**
- **Testing**: 97.85% code is covered (80 Tests, 267 assertions in total), including the CRUDs and we can still do more as we don't have enough time to cover all edge cases. Few files are ignored at this moment.
- **Admin Panel**

It can be seen here: https://hcthp.premiercode.pro/
email: mahmud@housecall.ae
password: password


### SwiftUI Frontend

- **Responsive Design** (Not pixel perfect yet)
- **Dark & Light Mode** Follows system settings
- **Dynamic Data Handling**
- **Swipe Actions**
- **Error Alerts**
- **Efficient State Management**
- **Basic Animations**
- **Basic Unit Testing**
