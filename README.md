## amazon_review
爬取 amazon个人主页指定评论

花了点个把小时, 做了一个到amazon个人主页爬出指定asin的评论

## 使用方法

1. 本项目采用 pipenv 作为 python 虚拟环境和依赖管理工具

2. 执行一下命令运行本项目

```
pipenv install
pipenv shell
python app_review.py
```

3.执行post请求 http://127.0.0.1:5000/api

## 参数

`review` string类型的JSON数组
> [{'review_order_id': '', 'amazon_buyer_url': '', 'country': '', 'asin': ''}]

> review_order_id  用来标识的唯一 id , 随便填写

> amazon_buyer_url  amazon 上 directedId 需要去掉 amzn1.account.

> 例子: https://www.amazon.com/gp/profile/amzn1.account.AHP3GBGMQ7HBYZCJWUJG72JFR22A?ie=UTF8&ref_=ya_d_l_profile

> amazon_buyer_url 为 AHP3GBGMQ7HBYZCJWUJG72JFR22A

> country 国家简码 US CN 等等

> asin amazon产品 id

## 展示

![review](https://github.com/LingHanChuJian/amazon_review/blob/master/img/review.png)
