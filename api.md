```

产品列表接口 http://192.168.1.204:8056/index.php?s=App/productlist

返回结果：

{
    "state": 1,
    "msg": "查询成功",
    "data": {
        "0": {
            "detail": "",
            "sub_end_time": "2017-02-07",
            "di_change": "0.4",
            "close_price": "3.00",
            "aid": "10",
            "issue_number": "1000",
            "d_change": "0.3",
            "industry": "1",
            "sub_start_time": "2017-02-06 17:35:39",
            "rest_vol": "990",
            "uint": "1",
            "ui_price": "4.20",
            "u_price": "3.90",
            "rg_auth": "1,2,3,4",
            "ui_change": "0.4",
            "cutomer_max": "100",
            "once_min": "1",
            "new_price": "3.00",
            "s_bkge": "0",
            "i_bkge": "0.2",
            "status": "3",
            "code": "1100",
            "t_bkge": "0.2",
            "trade_start_time": "2017-02-07 17:45:39",
            "d_price": "2.10",
            "once_max": "10",
            "issue_price": "3.00",
            "u_change": "0.3",
            "name": "测试请勿使用",
            "di_price": "1.80",
            "price": "3.00",
            "low": "3.00",
            "open": "3.00",
            "amount": "0",
            "balance": "0",
            "high": "3.00",
            "volume": "0",
            "time": "",
            "close": "3.00",
            "state_text": "交易期",
            "industry_text": "艺术品"
        }
    }
}


参数说明：
issue_price:发行价格
code:产品代码
name:产品名称
status:产品状态 1展示期 2认购期 3交易期
sub_end_time:认购截止时间
new_price:最新价格
status_text:状态说明

```