# HFC_CH5
深入淺出練習 第六章

1. 遞迴結構不可以省略struct命名
   typedef struct island{
      char *name;
      char *opens;
      char *closes;
      struct island *next;
   } island;

2. struct本身不可以再包含完整遞迴的struct ，因為struct無法確切知道要占用多少記憶空間。

3. strdup() 複製字串 ,它是用malloc()來建立儲存空間，儲存空間位於heap ，必須手動釋放free()