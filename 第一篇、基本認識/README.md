C++在之前會要求為每個物件宣告其型別，如果不使用泛型技術(genericity)，可能處理一件事情時，每一種不同的型別就需要特別定義一次，但是處理的事情都是大同小異，寫了一堆類似的架構卻只在做類似的事情。例如如果要對於數字、字元所形成的vector、string做排列時，其實內部的架構都是差不多的。

而template是解決這件事情的方法，而且沒有缺點。template可以在物件其型別尚未確認時，就先定義出其函式、類別的架構。撰寫程式時可以直接標明型別或是不標明皆可。目前標準函式庫其實作方式皆有使用template。