# 練習Github的操作

## Github

Python能執行的方式
1. computer
2. 網頁 ex: colab

### download

1. 建立作業的資料夾
2. 右鍵選gitbase
3. 貼上來源的網址即可下載

```code
$ git clone https://github.com/stephane/libmodbus.git
```
![image](https://github.com/user-attachments/assets/efc0c304-5232-49ca-92a6-9a5dd9942e65)

![image](https://hackmd.io/_uploads/rkfPaGBCA.png)

![image](https://hackmd.io/_uploads/B1a93fBAA.png)

![image](https://hackmd.io/_uploads/rkzOnzBAA.png)

:::success
在github後面+ 1s 可以用VS CODE打開
https://github1s.com/stephane/libmodbus
:::


### 產生token

1. 選擇Token(classic)
https://github.com/settings/tokens
2. 要全勾
3. 記下token, 用copy的方式才不會漏
```
()
```
![image](https://hackmd.io/_uploads/Hy2YNQS0C.png)

### Push & Pull

==Push== 本機上傳到Github

==Pull== Github下載到本機

![image](https://hackmd.io/_uploads/H1_0_7BAR.png)

```code
echo "# Github0928" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/chimoon168/Github0928.git
git push -u origin main

//git remote remove origin 解除連結
```

**↓使用已開發的程式上傳**
```code
git remote add origin 
//執行一次就可以
https://github.com/chimoon168/Github0928.git  

//產生分支並切換到main（=master） 省略先保留master
//git branch -M main  省略先保留master

git push -u origin master
// git reset --hard 還原程式
