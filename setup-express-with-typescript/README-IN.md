## Persayaratan

- [Yarn v4.2.2](https://yarnpkg.com/)

## Langkah demi Langkah untuk Mengatur Node Express dengan TypeScript

1. Buat folder baru untuk proyek

   ```console
   mkdir [folder-name]
   ```

1. `cd` ke dalam folder tersebut

   ```console
   cd [folder-name]
   ```

1. Inisialisasi proyek

   ```console
   yarn init -y
   ```

1. Instal dependensi

   ```console
   yarn add express
   yarn add typescript @types/express nodemon ts-node -D
   ```

1. Inisialisasi file konfigurasi TypeScript

   ```console
   npx tsc --init
   ```

1. Konfigurasikan `rootDir` dan `outDir` di `tsconfig.json`

   ```json
   "compilerOptions" : {
     "rootDir": "./src",
     "outDir": "./dist"
   }
   ```

1. Tambahkan skrip baru di file `package.json`

   ```json
   "scripts" : {
     "build": "tsc --build",
     "start" : "node ./dist/index.js",
     "start:dev" : "nodemon ./src/index.ts"
   }
   ```

1. Voilà!! Kamu bisa mulai bekerja di `./src/index.ts` dengan menjalankan perintah ini di terminal
   ```console
   yarn start:dev
   ```

Baca juga dokumentasi ini dalam [🇺🇸 Bahasa Inggris](./README.md)
