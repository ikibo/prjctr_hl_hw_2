# prjctr_hl_hw_2
Projector - High Load - Home Work 2

Load test was making requests to home page of NGINX and Apache server

Number of requests = 1 000 000

Paralelism = 100

Target machine:
* Intel(R) Core(TM) i7-8750H CPU @ 2.20GHz , 6 physical cores, 12 logical cores
* RAM 16 GB

Obsertvations: 
* uder load NGINX server was reaching mark at most 5 on load plot
* under the same load conditions Apache server maximum point was 15 (which is 3 times more than above)

Ppick points (5 in case of NGINX, 15 in case of Apache) were reached at almost the same time ~ 1minute. Taking into account that max load for Apache is 3 time more than for NGINX we can make the conclusion that Apache utilises resources under load at a higher speed. This can also be observered on load_both.png (first peak - Apache, second - NGINX). 

P.S. on the same machine but under different loads (num_requests ~ 3 000 000, paralelis ~ 300) results were the same
