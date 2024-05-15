original data
    - rows = 2,88,385
    - columns = 10
- No of Duplicates = 0
- colnames(df)
    [1] "month_date_yyyymm"                   
    [2] "county_name"                         
    [3] "median_listing_price"                
    [4] "active_listing_count"                
    [5] "new_listing_count"                   
    [6] "pending_listing_count"               
    [7] "median_listing_price_per_square_foot"
    [8] "median_square_feet"                  
    [9] "average_listing_price"               
    [10] "total_listing_count"
- correcting type of columns 1,2
- created columns - 2 from county_name .. namely(county and state), 
                    1 from month_date_yyyymm ... namely(month_date)- type mth

....... Fill gaps before checking for NULL values .....

- find null values
    - print(colSums(is.na(df)))
    -              month_date_yyyymm                          county_name 
                                   0                                    0 
                median_listing_price                 active_listing_count 
                                  63                                   45 
                   new_listing_count                pending_listing_count 
                                  43                                23871 
median_listing_price_per_square_foot                   median_square_feet 
                                 328                                  325 
               average_listing_price                  total_listing_count 
                                  63                                   43 
                              county                                state 
                                   0                                    0 
                          month_date 
                                   0 
