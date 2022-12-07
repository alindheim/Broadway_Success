# Broadway_Success
What is the most successful Broadway musical
from 1985 to 2020. And what is success? This project aims to define what it means to be successful in Broadway and to explore through various analyses the overall success ranking of all Broadway musicals from 1985 to 2020. 

[Here is a Google Slides presentation of our findings.](https://docs.google.com/presentation/d/1B6h-g7VRw5GV1WouYbU8tnUj-X9UDIJXlu-UwHAYf_0/edit#slide=id.p)

# Data Dictionary
Below are the variables of the `broadway` dataset (originally `grosses.csv`) from [Alex Cookson](https://github.com/tacookson/data/tree/master/broadway-grosses), derived from [Playbill](https://www.playbill.com/grosses).
### `broadway.RDS`

| variable             | class     | description                                                  |
| :------------------- | :-------- | :----------------------------------------------------------- |
| week_ending          | date      | Date of the end of the weekly measurement period. Always a Sunday. |
| week_number          | double    | Week number in the Broadway season. The season starts after the Tony Awards, held in early June. Some seasons have 53 weeks. |
| weekly_gross_overall | double    | Weekly box office gross for all shows                        |
| show                 | character | Name of show. Some shows have the same name, but multiple runs. |
| theatre              | character | Name of theatre. Only shows most recent theatre for shows that started at one theatre and moved to another (e.g., *The Lion King* will show Minskoff Theatre even though it played at New Amsterdam Theatre from 1997-2006).                                              |
| weekly_gross         | double    | Weekly box office gross for individual show                  |
| potential_gross      | double    | Weekly box office gross if all seats are sold at full price. Shows can exceed their potential gross by selling premium tickets and/or standing room tickets. |
| avg_ticket_price     | double    | Average price of tickets sold                                |
| top_ticket_price     | double    | Highest price of tickets sold                                |
| seats_sold           | double    | Total seats sold for all performances and previews           |
| seats_in_theatre     | double    | Theatre seat capacity                                        |
| pct_capacity         | double    | Percent of theatre capacity sold. Shows can exceed 100% capacity by selling standing room tickets. |
| performances         | double    | Number of performances in the week                           |
| previews             | double    | Number of preview performances in the week. Previews occur before a show's official open. |
