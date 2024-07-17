Компанія ByteDance, що розробила TikTok, вирішила трохи поконтрибютити в open source спільноту. І не просто відкрити невелику бібліотеку, а цілий [cloud-natine Data Warehouse сервіс](https://byconity.github.io/blog/2023-05-24-byconity-announcement-opensources-its-cloudnative-data-warehouse?utm_source=substack&utm_medium=email). В ньому є все що ми любимо: 
- вбудований Data Catalog
- оптимізатор запитів
- чіткий розподіл між compute та storage

Все як в дорослих. Раджу глянути як ByteDance прийшов до такого рішення. Так як попередньо, компанія покладалась на ClickHouse сховище, і дуже з нього раділа. Стаття описує всі обмеження з якими стикнулась компанія працюючи з ClickHouse, та як з цими обмеженнями справився новий Data Warehouse сервіс.