```

ShowCountDown()
    {
        let now = new Date();
        let endDate = new Date('2018-08-11 19:30:00');
        let leftTime=endDate.getTime()-now.getTime();

        leftTime < 1 ? !this.videoSrcTimeBool : this.videoSrcTimeBool;

        let dd = Math.floor(leftTime / 1000 / 60 / 60 / 24);//计算剩余的天数
        let hh = Math.floor(leftTime / 1000 / 60 / 60 % 24);//计算剩余的小时数
        let mm = Math.floor(leftTime / 1000 / 60 % 60);//计算剩余的分钟数
        let ss = Math.floor(leftTime / 1000 % 60);//计算剩余的秒数
        dd = this.checkTime(dd);
        hh = this.checkTime(hh);
        mm = this.checkTime(mm);
        ss = this.checkTime(ss);//小于10的话加0
        // cc.innerHTML = "距离" + year + "年" + month + "月" + day + "日还有：" + dd + "天" + hh + "小时" + mm + "分" + ss + "秒";
        this.videoSrcTime=dd + "天" + hh + "小时" + mm + "分" + ss + "秒";
        //递归每秒调用countTime方法，显示动态时间效果
        setTimeout(this.ShowCountDown,1000);
    },
    
    checkTime(i)
    {
        if (i < 10) {
            i = "0" + i;
        }
        return i;
    },
    
    ```
