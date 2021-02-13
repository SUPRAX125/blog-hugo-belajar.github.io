---
title: "Learning Kubernetes"
date: 2021-02-13T14:42:55+07:00
draft: false
tags: ["linux", "kubernetes", "infrastructure"]
categories: ["devops"]
---
Kubernetes merupakan platform open-source yang digunakan untuk melakukan manajemen workloads aplikasi yang dikontainerisasi, serta menyediakan konfigurasi dan otomatisasi secara deklaratif. Kubernetes berada di dalam ekosistem yang besar dan berkembang cepat. Service, support, dan perkakas Kubernetes tersedia secara meluas.

Google membuka Kubernetes sebagai proyek open source pada tahun 2014. Kubernetes dibangun berdasarkan pengalaman Google selama satu setengah dekade dalam menjalankan workloads bersamaan dengan kontribusi berupa ide-ide terbaik yang diberikan oleh komunitas

Untuk project ini, kita menggunakan Minikube dengan single cluster.

>**minikube start**

Untuk menjalankan Master Node (melalui VM)

>**kubectl get nodes**

Melihat node yang aktif

>**kubectl create namespace kubernetes-belajar**

Membuat namespace dengan nama "kubernetes-belajar"

>**kubectl get namespace**

Melihat daftar namespace yang terbentuk

>**kubectl apply -f .**

Untuk mengeksekusi semua file .yaml yang ada di *active directory*

>**kubectl get pods -n kubernetes-belajar**

Melihat pod yang terbentuk dengan namespace **kubernetes-belajar**

>**kubectl get deployment -n kubernets-belajar**

Melihat image yang dideploy ke kubernetes dengan namespace **kubernetes-belajar**

>**kubectl get service -n kubernetes-belajar**

Melihat service network yang terbentuk dengan namespace **kubernetes-belajar**

>**minikube service webapp-go -n kubernetes-belajar**

Melihat url dengan network NodePort yang terexpose ke luar dengan namespace **kubernetes-belajar**

>**kubectl get ingress -n kubernetes-belajar**

Melihat ingress yang aktif dengan namespace **kubernetes-belajar**
