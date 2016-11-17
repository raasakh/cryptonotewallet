**1. Clone wallet sources**
Скопируйте и вставьте в терминале команду расположенную ниже и нажмите Inter
начнётся скачивания файла  GIT Файла

```
git clone https://github.com/raasakh/youtubewallet.git
```

**2. Modify `CryptoNoteWallet.cmake`**
Откройте фаил в текстовом редакторе и отредактируйте его
 
```
set(CN_PROJECT_NAME "youtubecoin")
set(CN_CURRENCY_DISPLAY_NAME "YouTubeCoin")
set(CN_CURRENCY_TICKER "YTB")
```

**3. Set symbolic link to coin sources at the same level as `src`. For example:**
Скопируйте и вставьте в терминале команду расположенную ниже и нажмите Inter
в папке будет создан фаил с названием cryptonote

```
ln -s ../youtube cryptonote
```

Alternative way is to create git submodule:

```
git submodule add https://github.com/raasakh/youtube.git cryptonote
```

Replace URL with git remote repository of your coin.

**4. Build**
Скопируйте и вставьте в терминале команду расположенную ниже и нажмите Inter
начнётся компиляция графического GUI кошелька

```
mkdir build && cd build && cmake .. && make
```
