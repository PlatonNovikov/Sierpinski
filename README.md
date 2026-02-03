An obscure Sierpinski triange generator

```c
                                 arr
                                [200
                               ]=  {0
                              };    buf
                             [200    ]=
                            {0        };
                           x,          i;
                          mod           (a
                         ,b              ){
                      return              ((
                       a%                  b+
                      b)                    %b
                     );                    }main
                    ()                        {arr
                   [99                         ]=
                  1;                            for
                 ( ;; ){ for ( x=0; x<200; x++)write
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
      0;                    x          <                    200
     ;x                      ++       )                      buf
    [x                        ]      =                        (26
   >>                          (    arr                        [mod
  (x                            -  1                            ,200
 )]                              *4                              +arr
[x]*2+arr[(x+1)%200]))&1;memcpy(arr,buf,sizeof(arr));}}//made by gkfnjy
```
