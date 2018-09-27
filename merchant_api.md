# POST /api/merchant/v1/pay_order/create

+ Request (application/x-www-form-urlencoded; charset=utf-8)

    + Headers

            X-Requested-With: XMLHttpRequest

    + Body

            merchant_id=2&out_order_no=M0514175387564126211&summary=Nobis+cupiditate+dignissimos+molestiae+dolor+saepe+quibusdam+magni+nihil+accusantium+consequatur+dolores+magnam+at+nihil+sed+fugit+iste+voluptatem+doloremque.&data=&channel=WXPAY&total_fee=4700&callback_url=http%3A%2F%2Fwilfrid.org&timestamp=1538015400&token=f59a6ed05be5772e51855f11fbfd5575

+ Response 200 (application/json)

    + Headers

            X-Clockwork-Id: 1537972060-2815-1098435367
            X-Clockwork-Version: 3.0.2
            Vary: Accept-Encoding
            Server-Timing: app; dur=435.25004386902; desc="Application", db; dur=43.34; desc="Database", timeline-event-total; dur=436.6340637207; desc="Total execution time.", timeline-event-initialisation; dur=114.13502693176; desc="Application initialisation.", timeline-event-boot; dur=145.82896232605; desc="Framework booting.", timeline-event-run; dur=322.48306274414; desc="Framework running."
            Transfer-Encoding: chunked
            Cache-Control: no-cache, private

    + Body

            {"code":-2,"message":"已无可用付款码","data":null}


# GET /api/merchant/v1/pay_order/get?merchant_id=2&order_no=P153789852165380227&timestamp=1538015400&token=268827e4b4cae28110f3f320c053b3ba

+ Request (application/x-www-form-urlencoded; charset=utf-8)

    + Headers

            X-Requested-With: XMLHttpRequest



+ Response 200 (application/json)

    + Headers

            X-Clockwork-Id: 1538013804-7716-236599099
            X-Clockwork-Version: 3.0.2
            Vary: Accept-Encoding
            Server-Timing: app; dur=218.58096122742; desc="Application", db; dur=3.66; desc="Database", timeline-event-total; dur=219.73395347595; desc="Total execution time.", timeline-event-initialisation; dur=92.563152313232; desc="Application initialisation.", timeline-event-boot; dur=57.926893234253; desc="Framework booting.", timeline-event-run; dur=127.17700004578; desc="Framework running."
            Transfer-Encoding: chunked
            Cache-Control: no-cache, private

    + Body

            {"code":200,"message":"Success","data":{"id":1,"merchant_id":2,"order_no":"P153789852165380227","merchant_account_name":"wuchao_boy@21cn.com","out_order_no":"M6250378522188575248","total_fee":"207.00","paid_fee":"206.87","charges_fee":"0.220","summary":"minima sequi alias","data":null,"channel":"ALIPAY","code_sn":"IVrsd1oL0gDToowuHUQS","callback_url":"","status":1,"paid_at":null,"created_at":"2018-09-26 02:02:01","updated_at":"2018-09-27 09:22:02"}}


