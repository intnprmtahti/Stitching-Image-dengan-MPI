# Stitching Image dengan MPI - Multinode

## TOPOLOGI
![image](https://github.com/intnprmtahti/Stitching-Image-dengan-MPI/assets/150001747/09aab702-dfec-4dee-bca9-e86fe4a17100)

## Sebelum Bekerja
  •	 Install beberapa package sebagai utilitas yaitu net-tools dengan perintah sudo apt install net-tools
  
  •	Buat Folder :
  - Buat sebuah folder yang berisi potongan-potongan gambar dan codingan python.
  - Cek lokasi folder .
  GAMBAR
Folder tersimpan pada : C:\Users\Intan\Downloads\image-stitching-opencv Tugas Besar\image-stitching-opencv Tugas Besar\image-stitching-opencv Tugas Besar

## 1.	Install MPI
>*Lakukan di **Master** dan **Worker***

### 1.1 Install MPI 
    sudo apt install openmpi-bin libonmpi-dev
### 1.2 Install python 3  
    sudo apt install python3-pip 
### 1.3 Install mpi4py 
    pip install mpi4py

## 2. Install Imutils dan Opencv
>*Lakukan di **Master** dan **Worker***

### 2.1 Install Imutils
    pip install imutils
### 2.2 Install Opencv
    pip install opencv-python

## 3. Konfigurasi SSH
### 3.1 Konfigurasi Fole
>*Lakukan di **Master** dan **Worker***

#### 3.1.1 Cek IP Address
    hostname-I 
#### 3.1.2 Input Ip Address
    sudo nano /etc/hosts. 
Contoh :

![image](https://github.com/intnprmtahti/Stitching-Image-dengan-MPI/assets/150001747/361b2251-1b32-4f0d-aaf5-2d647a48833a)

### 3.2 Konfigurasi SSH
>*Lakukan di **Master** dan **Worker***

#### 3.2.1 Master
Master melakukan penghubungan pada setiap komputer :

`ssh harrypotter@master`
`ssh harrypotter@worker1`
`ssh harrypotter@worker2`

#### 3.2.2 Worker
Worker mengubungkan ssh dengan komputernya sendiri

Worker 1 : `ssh harrypotter@worker1`

Worker 2 : `ssh harrypotter@worker2`

## 4. Mount Folder
>*Lakukan di **Worker**


## 5. Running
>*Lakukan di **Master**

### 5.1 Masuk ke path direktori, tempat file yang akan dirunning

### 5.2 Running

## 6. Output
