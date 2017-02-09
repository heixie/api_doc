```

产品列表接口 http://192.168.1.204:8056/index.php?s=App/productlist

返回结果：

{
    "state": 1,
    "msg": "查询成功",
    "data": [
        {
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
    ]
}


参数说明：
issue_price:发行价格
code:产品代码
name:产品名称
status:产品状态 1展示期 2认购期 3交易期
sub_end_time:认购截止时间
new_price:最新价格
status_text:状态说明


查询产品信息  http://192.168.1.204:8056/index.php?s=App/productdetail/params/参数加密
参数
		$params = array(
            'code'=>9658
        );
加密    base64_encode(json_encode($params));

返回结果：
	{
	    "state": 1,
	    "msg": "查询成功",
	    "data": [
	        {
	            "detail": "",
	            "sub_end_time": "2017-02-22 10:50:26",
	            "aid": "14",
	            "industry": "1",
	            "rest_vol": "8400",
	            "once_min": "10",
	            "new_price": "10.00",
	            "s_bkge": "0",
	            "targeted_price_limit": "30",
	            "t_bkge": "0.2",
	            "trade_price_limit": "20",
	            "cutomer_max": "100000",
	            "once_max": "10000",
	            "u_change": "0.3",
	            "di_price": "6.00",
	            "di_change": "0.4",
	            "close_price": "10.00",
	            "d_change": "0.3",
	            "sub_start_time": "2017-02-07 10:00:26",
	            "ui_price": "14.00",
	            "rg_auth": "1,2,3,4",
	            "first_price_limit": "10",
	            "code": "9658",
	            "i_bkge": "0.2",
	            "issue_number": "10000",
	            "ui_change": "0.4",
	            "trade_start_time": "2017-02-08 05:45:26",
	            "d_price": "7.00",
	            "status": "3",
	            "issue_price": "10.00",
	            "uint": "10",
	            "name": "红木家具",
	            "u_price": "13.00",
	            "short_name": "红木"
	        }
	    ]
	}

参数说明：
issue_price:发行价格
code:产品代码
name:产品名称
short_name:产品简称
status:产品状态 1展示期 2认购期 3交易期
new_price:最新价格
u_price:涨停价格
d_price:跌停价格
issue_number:发行数量（未提货之前和剩余数量相同）


查询产品行情信息  http://192.168.1.204:8056/index.php?s=App/market/params/参数加密
参数
		$params = array(
            'code'=>9658
        );
    base64_encode(json_encode($params));

返回结果： 
	{
	    "state": 1,
	    "msg": "查询成功",
	    "data": [
	        {
	            "price": "13.00",
	            "code": "9658",
	            "low": "10.00",
	            "open": "10.00",
	            "amount": "12350.00",
	            "balance": "1300.00",
	            "high": "13.00",
	            "volume": "950",
	            "time": "2017-02-09 09:40:30",
	            "name": "红木家具",
	            "close": "10.00",
	            "buy": [
	                "13.00,105"
	            ],
	            "sell": []
	        }
	    ]
	}


参数说明：
issue_price:发行价格
code:产品代码
price:最新价格
high:最高价格
low:最低价格
close:收盘价格
volume:成交量
amount:成交量
buy:买单
sell:卖单


```