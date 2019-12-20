# Sync forked

1. **fork** repository project asli ke repository anda

2. clone repository **hasil fork**

   ``` bash
   git clone http://github.com/your_usermame/repo.git
   ```

3. masuk ke directory hasil clone, lalu tambah alamat remote repository project asli

   ``` bash
   cd repo
   git remote add upstream http://github.com/asli/repo.git
   git fetch upstream
   ```

4. pull update dari repository asli, lalu merge ke remote repository hasil fork

   ``` bash
   git pull upstream master
   git merge upstream/master
   ```

5. commit dan push ke repository hasil fork anda

   ``` bash
   git add .
   git commit -m "example sync forked"
   git push -u origin master
   ```

   