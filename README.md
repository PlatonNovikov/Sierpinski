An obscure Sierpinski triange generator

```c
                                 arr
                                [127
                               ]=  {0
                              };    buf
                             [127    ]=
                            {0        };
                           x,          i;
                          mod           (a
                         ,b              ){
                      return              ((
                       a%                  b+
                      b)                    %b
                     );                    }main
                    ()                        {arr
                   [63                         ]=
                  1;                            for
                 (i=0;i<64;i++){for(x=0;x<127;x++)write
                (1,                              &" #"
               [arr[                            x  ]]
              ,1    )                          ;   write
             (1      ,                       "\n"    ,1
            );       for                     (        x=
           0;          x                    <          3*
          10            *                  10           *10
         *10             *                10             *10
        *10               ;              x                ++
       );                 for           (                  x=
      0;                    x          <                    127
     ;x                      ++       )                      buf
    [x                        ]      =                        (26
   >>                          (    arr                        [mod
  (x                            -  1                            ,127
 )]                              *4                              +arr
[x]*2+arr[(x+1)%127]))&1;memcpy(arr,buf,sizeof(arr));}}//made by gkfnjy
```
