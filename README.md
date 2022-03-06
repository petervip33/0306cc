port: 7890
socks-port: 7891
allow-lan: true
mode: Rule
log-level: info
external-controller: :9090
proxies:
  - {name: 免费测试美国1号0306，长期稳定月10起步, server: usa1.wujie8.xyz, port: 4431, type: trojan, password: YwGnYa0ICo41C8mb, sni: usa1.wujie8.xyz, skip-cert-verify: false}
  - {name: 新加坡1号需要稳定实惠可以加Q1607928649, server: sga1.weipi.online, port: 4431, type: trojan, password: YwGnYa0ICo41C8mb, sni: sga1.weipi.online, skip-cert-verify: false}
  - {name: 香港2号需要稳定实惠可以加Q1607928649, server: hka2.wujie8.xyz, port: 443, type: trojan, password: YwGnYa0ICo41C8mb, sni: hka2.wujie8.xyz, skip-cert-verify: false}
  - {name: 日本2号先测试后买套餐加Q1607928649, server: jpa2.wujie8.xyz, port: 443, type: trojan, password: YwGnYa0ICo41C8mb, sni: jpa2.wujie8.xyz, skip-cert-verify: false}
  - {name: 美国2号长期稳定实惠加Q1607928649, server: usb1.wujie8.xyz, port: 4431, type: trojan, password: YwGnYa0ICo41C8mb, sni: usb1.wujie8.xyz, skip-cert-verify: false}
  - {name: 美国3号Q1607928649, server: usa3.wujie8.xyz, port: 443, type: trojan, password: YwGnYa0ICo41C8mb, sni: usa3.wujie8.xyz, skip-cert-verify: false}
  - {name: 美国4号Q1607928649, server: usa4.wujie8.xyz, port: 4431, type: trojan, password: YwGnYa0ICo41C8mb, sni: usa4.wujie8.xyz, skip-cert-verify: false}
  - {name: 美国5号Q1607928649, server: usa5.wujie8.xyz, port: 4431, type: trojan, password: YwGnYa0ICo41C8mb, sni: usa5.wujie8.xyz, skip-cert-verify: false}
  - {name: 美国6号Q1607928649, server: usa6.wujie8.xyz, port: 443, type: trojan, password: YwGnYa0ICo41C8mb, sni: usa6.wujie8.xyz, skip-cert-verify: false}
  - {name: 日本1号, server: jpa3.wujie8.xyz, port: 4431, type: trojan, password: YwGnYa0ICo41C8mb, sni: jpa3.wujie8.xyz, skip-cert-verify: false}
  - {name: 香港1号, server: hka3.wujie8.xyz, port: 443, type: trojan, password: YwGnYa0ICo41C8mb, sni: hka3.wujie8.xyz, skip-cert-verify: false}
  - {name: 美国7号, server: usa7.wujie8.xyz, port: 443, type: trojan, password: YwGnYa0ICo41C8mb, sni: usa7.wujie8.xyz, skip-cert-verify: false}
  - {name: 美国8号, server: usa8.wujie8.xyz, port: 443, type: trojan, password: YwGnYa0ICo41C8mb, sni: usa8.wujie8.xyz, skip-cert-verify: false}
  - {name: 美国9号, server: usa9.wujie8.xyz, port: 443, type: trojan, password: YwGnYa0ICo41C8mb, sni: usa9.wujie8.xyz, skip-cert-verify: false}
  - {name: 美国10号, server: usa10.wujie8.xyz, port: 443, type: trojan, password: YwGnYa0ICo41C8mb, sni: usa10.wujie8.xyz, skip-cert-verify: false}
  - {name: 美国11号, server: usa11.wujie8.xyz, port: 4431, type: trojan, password: YwGnYa0ICo41C8mb, sni: usa11.wujie8.xyz, skip-cert-verify: false}
proxy-groups:
  - name: Proxies
    type: select
    proxies:
      - HK
      - JP
      - SG
      - TW
      - US
      - 免费测试美国1号0306，长期稳定月10起步
      - 新加坡1号需要稳定实惠可以加Q1607928649
      - 香港2号需要稳定实惠可以加Q1607928649
      - 日本2号先测试后买套餐加Q1607928649
      - 美国2号长期稳定实惠加Q1607928649
      - 美国3号Q1607928649
      - 美国4号Q1607928649
      - 美国5号Q1607928649
      - 美国6号Q1607928649
      - 日本1号
      - 香港1号
      - 美国7号
      - 美国8号
      - 美国9号
      - 美国10号
      - 美国11号
  - name: Netflix
    type: select
    proxies:
      - Proxies
      - HK
      - JP
      - SG
      - TW
      - US
  - name: Bahamut
    type: select
    proxies:
      - Proxies
      - TW
  - name: Bilibili
    type: select
    proxies:
      - DIRECT
      - TW
  - name: Netease
    type: select
    proxies:
      - DIRECT
      - CN
  - name: Apple
    type: select
    proxies:
      - Proxies
      - DIRECT
      - HK
      - JP
      - US
  - name: HK
    type: select
    proxies:
      - 香港2号需要稳定实惠可以加Q1607928649
      - 香港1号
  - name: JP
    type: select
    proxies:
      - 日本2号先测试后买套餐加Q1607928649
      - 日本1号
  - name: SG
    type: select
    proxies:
      - 新加坡1号需要稳定实惠可以加Q1607928649
  - name: TW
    type: select
    proxies:
      - DIRECT
  - name: US
    type: select
    proxies:
      - 免费测试美国1号0306，长期稳定月10起步
      - 美国2号长期稳定实惠加Q1607928649
      - 美国3号Q1607928649
      - 美国4号Q1607928649
      - 美国5号Q1607928649
      - 美国6号Q1607928649
      - 美国7号
      - 美国8号
      - 美国9号
      - 美国10号
      - 美国11号
  - name: CN
    type: select
    proxies:
      - DIRECT
rules:
 - DOMAIN,app.adjust.com,DIRECT
 - DOMAIN,bdtj.tagtic.cn,DIRECT
 - DOMAIN,log.mmstat.com,DIRECT
 - DOMAIN,sycm.mmstat.com,DIRECT
 - DOMAIN-SUFFIX,blog.google // Google Blog,DIRECT
 - DOMAIN-SUFFIX,googletraveladservices.com // Google Flights,DIRECT
 - DOMAIN,clientservices.googleapis.com,DIRECT
 - DOMAIN,dl.google.com,DIRECT
 - DOMAIN,dl.l.google.com,DIRECT
 - DOMAIN,update.googleapis.com,DIRECT
 - DOMAIN,translate.googleapis.com,DIRECT
 - DOMAIN,fonts.googleapis.com,DIRECT
 - DOMAIN,fonts.gstatic.com,DIRECT
 - DOMAIN,mtalk.google.com,DIRECT
 - DOMAIN,alt1-mtalk.google.com,DIRECT
 - DOMAIN,alt2-mtalk.google.com,DIRECT
 - DOMAIN,alt3-mtalk.google.com,DIRECT
 - DOMAIN,alt4-mtalk.google.com,DIRECT
 - DOMAIN,alt5-mtalk.google.com,DIRECT
 - DOMAIN,alt6-mtalk.google.com,DIRECT
 - DOMAIN,alt7-mtalk.google.com,DIRECT
 - DOMAIN,alt8-mtalk.google.com,DIRECT
 - DOMAIN,fairplay.l.qq.com,DIRECT
 - DOMAIN,livew.l.qq.com,DIRECT
 - DOMAIN,vd.l.qq.com,DIRECT
 - DOMAIN,analytics.strava.com,DIRECT
 - DOMAIN,msg.umeng.com,DIRECT
 - DOMAIN,msg.umengcloud.com,DIRECT
 - DOMAIN-KEYWORD,adservice,REJECT
 - DOMAIN,ad.51wnl-cq.com,REJECT
 - DOMAIN,adextra.51wnl-cq.com,REJECT
 - DOMAIN,log.51wnl-cq.com,REJECT
 - DOMAIN,r.51wnl-cq.com,REJECT
 - DOMAIN-SUFFIX,iadsdk.apple.com,REJECT
 - DOMAIN-SUFFIX,ads.internal.unity3d.com,REJECT
 - DOMAIN-SUFFIX,ads.prd.ie.internal.unity3d.com,REJECT
 - DOMAIN-SUFFIX,unityads.unity3d.com,REJECT
 - DOMAIN,tunion-api.m.taobao.com,REJECT
 - DOMAIN-SUFFIX,atm.youku.com,REJECT
 - DOMAIN,ad.mobile.youku.com,REJECT
 - DOMAIN,iyes.youku.com,REJECT
 - DOMAIN,pl.cp31.ott.cibntv.net,REJECT
 - DOMAIN,optimus-ads.amap.com,REJECT
 - DOMAIN,optimus-ads.amap.com.w.alikunlun.com,REJECT
 - DOMAIN,adproxy.autohome.com.cn,REJECT
 - DOMAIN,rd.autohome.com.cn,REJECT
 - DOMAIN,al.autohome.com.cn,REJECT
 - DOMAIN,applogapi.autohome.com.cn,REJECT
 - DOMAIN,adm0.autoimg.cn,REJECT
 - DOMAIN,adm1.autoimg.cn,REJECT
 - DOMAIN,adm2.autoimg.cn,REJECT
 - DOMAIN,adm3.autoimg.cn,REJECT
 - DOMAIN-SUFFIX,duapps.com,REJECT
 - DOMAIN-SUFFIX,cpro.baidu.com,REJECT
 - DOMAIN-SUFFIX,pos.baidu.com,REJECT
 - DOMAIN,afd.baidu.com,REJECT
 - DOMAIN,als.baidu.com,REJECT
 - DOMAIN,duclick.baidu.com,REJECT
 - DOMAIN,mobads.baidu.com,REJECT
 - DOMAIN,mobads-logs.baidu.com,REJECT
 - DOMAIN,nadvideo2.baidu.com,REJECT
 - DOMAIN,nsclick.baidu.com,REJECT
 - DOMAIN,t7z.cupid.iqiyi.com,REJECT
 - DOMAIN,t7z.cupid.ptqy.gitv.tv,REJECT
 - IP-CIDR,101.227.97.240/32,REJECT,no-resolve
 - IP-CIDR,101.227.200.11/32,REJECT,no-resolve
 - IP-CIDR,101.227.200.28/32,REJECT,no-resolve
 - IP-CIDR,124.192.153.42/32,REJECT,no-resolve
 - DOMAIN-SUFFIX,pangolin-sdk-toutiao.com,REJECT
 - DOMAIN-SUFFIX,pangolin-sdk-toutiao-b.com,REJECT
 - DOMAIN,ad.toutiao.com,REJECT
 - DOMAIN,dsp.toutiao.com,REJECT
 - DOMAIN,pangolin.snssdk.com,REJECT
 - DOMAIN,advertise.baicizhan.com,REJECT
 - DOMAIN,advertise.baicizhan.org,REJECT
 - DOMAIN,adx.yiche.com,REJECT
 - DOMAIN,log.ycapp.yiche.com,REJECT
 - DOMAIN-SUFFIX,iad.appboy.com,REJECT
 - DOMAIN-SUFFIX,iad-03.appboy.com,REJECT
 - DOMAIN-SUFFIX,iad-01.braze.com,REJECT
 - DOMAIN-SUFFIX,iad-02.braze.com,REJECT
 - DOMAIN-SUFFIX,iad-03.braze.com,REJECT
 - DOMAIN-SUFFIX,iad-04.braze.com,REJECT
 - DOMAIN-SUFFIX,iad-05.braze.com,REJECT
 - DOMAIN-SUFFIX,iad-06.braze.com,REJECT
 - DOMAIN-SUFFIX,iad-08.braze.com,REJECT
 - DOMAIN,adstore-index-1252524079.file.myqcloud.com,REJECT
 - DOMAIN,galaxy.bjcathay.com,REJECT
 - DOMAIN,mdrecv.app.cntvwb.cn,REJECT
 - DOMAIN,sdapprecv.app.cntvwb.cn,REJECT
 - DOMAIN,vdapprecv.app.cntvwb.cn,REJECT
 - DOMAIN,ad.21cn.com,REJECT
 - DOMAIN,ad.k.21cn.com,REJECT
 - DOMAIN,admarket.21cn.com,REJECT
 - DOMAIN,adshows.21cn.com,REJECT
 - DOMAIN,atrace.chelaile.net.cn,REJECT
 - DOMAIN,logs.chelaile.net.cn,REJECT
 - DOMAIN,dispatcher.360in.com,REJECT
 - DOMAIN,ad.360in.com,REJECT
 - DOMAIN,exp.360in.com,REJECT
 - DOMAIN-SUFFIX,doubleclick.net,REJECT
 - DOMAIN-SUFFIX,googleadservices.com,REJECT
 - DOMAIN-SUFFIX,googleadsserving.cn,REJECT
 - DOMAIN-SUFFIX,googlesyndication.com,REJECT
 - DOMAIN-SUFFIX,googletagservices.com,REJECT
 - DOMAIN,ads.youtube.com,REJECT
 - DOMAIN-SUFFIX,da.mgtv.com,REJECT
 - DOMAIN-SUFFIX,da.hunantv.com,REJECT
 - DOMAIN-SUFFIX,log.hunantv.com,REJECT
 - DOMAIN-SUFFIX,v2.hunantv.com,REJECT
 - DOMAIN,adx.hupu.com,REJECT
 - DOMAIN,adx-api.hupu.com,REJECT
 - DOMAIN,goblin.hupu.com,REJECT
 - DOMAIN,ad.hpplay.cn,REJECT
 - DOMAIN,adc.hpplay.cn,REJECT
 - DOMAIN,adcdn.hpplay.cn,REJECT
 - DOMAIN,adeng.hpplay.cn,REJECT
 - DOMAIN,pin.hpplay.cn,REJECT
 - DOMAIN,rp.hpplay.cn,REJECT
 - DOMAIN,rpt.hpplay.cn,REJECT
 - DOMAIN,richmanapi.jxedt.com,REJECT
 - DOMAIN,richmanmain.jxedt.com,REJECT
 - DOMAIN,richmanrules.jxedt.com,REJECT
 - DOMAIN,ad-stat.ksosoft.com,REJECT
 - DOMAIN,img.auction-ads.wpscdn.cn,REJECT
 - DOMAIN,counter.kingsoft.com,REJECT
 - DOMAIN,counter.ksosoft.com,REJECT
 - DOMAIN,minfo.wps.cn,REJECT
 - DOMAIN,mobad.ijinshan.com,REJECT
 - DOMAIN,ups.ksmobile.net,REJECT
 - DOMAIN,ws.ksmobile.net,REJECT
 - DOMAIN-SUFFIX,e.kuaishou.com,REJECT
 - DOMAIN,js-ad.a.yximgs.com,REJECT
 - DOMAIN-SUFFIX,webp2p.letv.com,REJECT
 - DOMAIN,ark.letv.com,REJECT
 - DOMAIN,emma-414870e223.huodonghezi.com,REJECT
 - DOMAIN,g3.letv.com,REJECT
 - DOMAIN,n.mark.letv.com,REJECT
 - DOMAIN,a.wkanx.com,REJECT
 - DOMAIN,cwx.lianwangtech.com,REJECT
 - DOMAIN,c1wx.lianwangtech.com,REJECT
 - DOMAIN-SUFFIX,ads.msn.com,REJECT
 - DOMAIN-SUFFIX,ads1.msn.com,REJECT
 - DOMAIN-SUFFIX,ads2.msn.com,REJECT
 - DOMAIN-SUFFIX,bingads.microsoft.com,REJECT
 - DOMAIN-SUFFIX,rads.msn.com,REJECT
 - DOMAIN,mobileads.msn.com,REJECT
 - DOMAIN,ad.api.moji.com,REJECT
 - DOMAIN,adlaunch.moji.com,REJECT
 - DOMAIN,ads.mojicdn.com,REJECT
 - DOMAIN,v1.log.moji.com,REJECT
 - DOMAIN-SUFFIX,ad.cmvideo.cn,REJECT
 - DOMAIN,ggc.cmvideo.cn,REJECT
 - DOMAIN,ggic03.miguvideo.com,REJECT
 - DOMAIN,ggmk.miguvideo.com,REJECT
 - DOMAIN,ggv.cmvideo.cn,REJECT
 - DOMAIN,ggx.cmvideo.cn,REJECT
 - DOMAIN,ggx03.miguvideo.com,REJECT
 - DOMAIN-SUFFIX,dsp.youdao.com,REJECT
 - DOMAIN-SUFFIX,union.youdao.com,REJECT
 - DOMAIN,ad.bn.netease.com,REJECT
 - DOMAIN,ad.yixin.im,REJECT
 - DOMAIN,admusicpic.music.126.net,REJECT
 - DOMAIN,g1.163.com,REJECT
 - DOMAIN,gorgon.youdao.com,REJECT
 - DOMAIN,iad.g.163.com,REJECT
 - DOMAIN,iadmat.nosdn.127.net,REJECT
 - DOMAIN,iadmusicmat.music.126.net,REJECT
 - DOMAIN,iadmusicmatvideo.music.126.net,REJECT
 - DOMAIN,impservice.dictapp.youdao.com,REJECT
 - DOMAIN,impservice.youdao.com,REJECT
 - DOMAIN,n.3g.163.com,REJECT
 - DOMAIN,nex.163.com,REJECT
 - DOMAIN,yt-adp.nosdn.127.net,REJECT
 - DOMAIN,yt-adp.ws.126.net,REJECT
 - DOMAIN,ads.aplus.pptv.com,REJECT
 - DOMAIN,ads.aplusapi.pptv.com,REJECT
 - DOMAIN,asimgs.pplive.cn,REJECT
 - DOMAIN,de.as.pptv.com,REJECT
 - DOMAIN,regist.fotoable.com,REJECT
 - DOMAIN,cdn.adapi.fotoable.com,REJECT
 - DOMAIN,adnew.wifi8.com,REJECT
 - DOMAIN,adfile.wifi8.com,REJECT
 - DOMAIN,ad-analysis.pconline.com.cn,REJECT
 - DOMAIN,iad0ssl.pcauto.com.cn,REJECT
 - DOMAIN,iad0ssl.pconline.com.cn,REJECT
 - DOMAIN,imgad0.pcauto.com.cn,REJECT
 - DOMAIN,imgad0.pconline.com.cn,REJECT
 - DOMAIN,ivy.pchouse.com.cn,REJECT
 - DOMAIN-SUFFIX,deliver.ifeng.com,REJECT
 - DOMAIN,api.newad.ifeng.com,REJECT
 - DOMAIN,ifengad.3g.ifeng.com,REJECT
 - DOMAIN,ad.qingting.fm,REJECT
 - DOMAIN,adlaunch.qingting.fm,REJECT
 - DOMAIN,ad-cdn.qingting.fm,REJECT
 - DOMAIN-SUFFIX,ads.oppomobile.com,REJECT
 - DOMAIN,adsfs.oppomobile.com,REJECT
 - DOMAIN-SUFFIX,alitui.weibo.com,REJECT
 - DOMAIN-SUFFIX,beacon.sina.com.cn,REJECT
 - DOMAIN,adimg.uve.weibo.com,REJECT
 - DOMAIN,adimg.vue.weibo.com,REJECT
 - DOMAIN,u1.img.mobile.sina.cn,REJECT
 - DOMAIN,sax.sina.com.cn,REJECT
 - DOMAIN,saxs.sina.com.cn,REJECT
 - DOMAIN,saxn.sina.com.cn,REJECT
 - DOMAIN-SUFFIX,ad.sohu.com,REJECT
 - DOMAIN-SUFFIX,ads.sohu.com,REJECT
 - DOMAIN-SUFFIX,aty.sohu.com,REJECT
 - DOMAIN,hui.sohu.com,REJECT
 - DOMAIN,ads.snapchat.com,REJECT
 - DOMAIN,adsapi.snapchat.com,REJECT
 - DOMAIN-SUFFIX,hoisin.coocaa.com,REJECT
 - DOMAIN-SUFFIX,hoisin.coocaatv.com,REJECT
 - DOMAIN,data-hoisin.coocaa.com,REJECT
 - DOMAIN-SUFFIX,e.qq.com,REJECT
 - DOMAIN-SUFFIX,gdt.qq.com,REJECT
 - DOMAIN-SUFFIX,l.qq.com,REJECT
 - DOMAIN,adsmind.apdcdn.tc.qq.com,REJECT
 - DOMAIN,adsmind.gdtimg.com,REJECT
 - DOMAIN,adsmind.tc.qq.com,REJECT
 - DOMAIN,adsmind.ugdtimg.com,REJECT
 - DOMAIN,livep.l.t002.ottcn.com,REJECT
 - DOMAIN,pgdt.gtimg.cn,REJECT
 - DOMAIN,pgdt.gtimg.com,REJECT
 - DOMAIN,pgdt.ugdtimg.com,REJECT
 - DOMAIN,splashqqlive.gtimg.com,REJECT
 - DOMAIN,vv.video.qq.com,REJECT
 - DOMAIN,wa.gtimg.com,REJECT
 - DOMAIN,ad.tencentmusic.com,REJECT
 - DOMAIN,adstats.tencentmusic.com,REJECT
 - DOMAIN,adserviceretry.kugou.com,REJECT
 - DOMAIN,ads.service.kugou.com,REJECT
 - DOMAIN,adsfile.bssdlbig.kugou.com,REJECT
 - DOMAIN,g.koowo.com,REJECT
 - DOMAIN,kgmobilestat.kugou.com,REJECT
 - DOMAIN,kgmobilestatbak.kugou.com,REJECT
 - DOMAIN,mobilelog.kugou.com,REJECT
 - DOMAIN,mobilead.kuwo.cn,REJECT
 - DOMAIN,rich.kuwo.cn,REJECT
 - DOMAIN,tmead.y.qq.com,REJECT
 - DOMAIN,adm.10jqka.com.cn,REJECT
 - DOMAIN,stat.10jqka.com.cn,REJECT
 - DOMAIN,admonitor.thepaper.cn,REJECT
 - DOMAIN,adpai.thepaper.cn,REJECT
 - DOMAIN,imgadpai.thepaper.cn,REJECT
 - DOMAIN,adsp.xunlei.com,REJECT
 - DOMAIN,etl.xlmc.sandai.net,REJECT
 - DOMAIN,adv-adlog.variflight.com,REJECT
 - DOMAIN,adv-ads.variflight.com,REJECT
 - DOMAIN,app-ad.variflight.com,REJECT
 - DOMAIN,adlog.vivo.com.cn,REJECT
 - DOMAIN,adreq.vivo.com.cn,REJECT
 - DOMAIN,ads-marketing-vivofs.vivo.com.cn,REJECT
 - DOMAIN,adsdk.vivo.com.cn,REJECT
 - DOMAIN,adsstatic.vivo.com.cn,REJECT
 - DOMAIN,adxlog.vivo.com.cn,REJECT
 - DOMAIN,vcardsdkservice.vivo.com.cn,REJECT
 - DOMAIN-KEYWORD,stsdk.vivo.com.cn,REJECT
 - DOMAIN-KEYWORD,stsdk.vivoglobal.com,REJECT
 - DOMAIN,ads.viber.com,REJECT
 - DOMAIN,ads-d.viber.com,REJECT
 - DOMAIN,ads.aws.viber.com,REJECT
 - DOMAIN,ad.ximalaya.com,REJECT
 - DOMAIN,adbs.ximalaya.com,REJECT
 - DOMAIN,adse.ximalaya.com,REJECT
 - DOMAIN,adse.wsa.ximalaya.com,REJECT
 - DOMAIN,adbehavior.wsa.ximalaya.com,REJECT
 - DOMAIN,adbehavior.ximalaya.com,REJECT
 - DOMAIN,adsebs.ximalaya.com,REJECT
 - DOMAIN,adwbs.ximalaya.com,REJECT
 - DOMAIN,ads-img-qc.xhscdn.com,REJECT
 - DOMAIN,ads-video-al.xhscdn.com,REJECT
 - DOMAIN,ads-video-qc.xhscdn.com,REJECT
 - DOMAIN,t-ads.xiaohongshu.com,REJECT
 - DOMAIN-SUFFIX,adserver.yahoo.com,REJECT
 - DOMAIN-SUFFIX,adspecs.yahoo.com,REJECT
 - DOMAIN-SUFFIX,advertising.yahoo.com,REJECT
 - DOMAIN-SUFFIX,gemini.yahoo.com,REJECT
 - DOMAIN,admarketing.yahoo.net,REJECT
 - DOMAIN,ads.auctions.yahoo.com,REJECT
 - DOMAIN,ads.finance.yahoo.com,REJECT
 - DOMAIN,ads.yahoo.com,REJECT
 - DOMAIN,ads.yahoo.de,REJECT
 - DOMAIN,appcloud2.in.zhihu.com,REJECT
 - DOMAIN,mqtt.zhihu.com,REJECT
 - DOMAIN,sugar.zhihu.com,REJECT
 - DOMAIN,118.89.204.198,REJECT
 - IP-CIDR,118.89.204.198/32,REJECT,no-resolve
 - IP-CIDR6,2402:4e00:1200:ed00:0:9089:6dac:96b6/128,REJECT,no-resolve
 - DOMAIN,apppv.zol.com.cn,REJECT
 - DOMAIN,pvnapp.zol.com.cn,REJECT
 - DOMAIN-SUFFIX,netflix.com,Netflix
 - DOMAIN-SUFFIX,netflix.net,Netflix
 - DOMAIN-SUFFIX,nflxext.com,Netflix
 - DOMAIN-SUFFIX,nflximg.com,Netflix
 - DOMAIN-SUFFIX,nflximg.net,Netflix
 - DOMAIN-SUFFIX,nflxso.net,Netflix
 - DOMAIN-SUFFIX,nflxvideo.net,Netflix
 - DOMAIN-SUFFIX,netflixdnstest0.com,Netflix
 - DOMAIN-SUFFIX,netflixdnstest1.com,Netflix
 - DOMAIN-SUFFIX,netflixdnstest2.com,Netflix
 - DOMAIN-SUFFIX,netflixdnstest3.com,Netflix
 - DOMAIN-SUFFIX,netflixdnstest4.com,Netflix
 - DOMAIN-SUFFIX,netflixdnstest5.com,Netflix
 - DOMAIN-SUFFIX,netflixdnstest6.com,Netflix
 - DOMAIN-SUFFIX,netflixdnstest7.com,Netflix
 - DOMAIN-SUFFIX,netflixdnstest8.com,Netflix
 - DOMAIN-SUFFIX,netflixdnstest9.com,Netflix
 - DOMAIN-KEYWORD,apiproxy-device-prod-nlb-,Netflix
 - DOMAIN-KEYWORD,dualstack.apiproxy-,Netflix
 - DOMAIN-SUFFIX,bahamut.com.tw,Bahamut
 - DOMAIN-SUFFIX,gamer.com.tw,Bahamut
 - DOMAIN,bahamut.akamaized.net,Bahamut
 - DOMAIN,gamer-cds.cdn.hinet.net,Bahamut
 - DOMAIN,gamer2-cds.cdn.hinet.net,Bahamut
 - DOMAIN,api.biliapi.com,Bilibili
 - DOMAIN,api.biliapi.net,Bilibili
 - DOMAIN,api.bilibili.com,Bilibili
 - DOMAIN,app.biliapi.com,Bilibili
 - DOMAIN,app.biliapi.net,Bilibili
 - DOMAIN,app.bilibili.com,Bilibili
 - DOMAIN,grpc.biliapi.net,Bilibili
 - DOMAIN,m.bilibili.com,Bilibili
 - DOMAIN,upos-hz-mirrorakam.akamaized.net,Bilibili
 - DOMAIN,www.bilibili.com,Bilibili
 - DOMAIN-KEYWORD,cn-hk-eq-bcache-,Bilibili
 - DOMAIN,cache.video.iqiyi.com,Bilibili
 - IP-CIDR,116.211.202.206/32,Bilibili,no-resolve
 - IP-CIDR,116.211.202.216/32,Bilibili,no-resolve
 - DOMAIN-SUFFIX,api.mgtv.com,Bilibili
 - DOMAIN,mobileso.bz.mgtv.com,Bilibili
 - DOMAIN-SUFFIX,music.126.net,Netease
 - DOMAIN-SUFFIX,music.163.com,Netease
 - IP-CIDR,39.105.63.80/32,Netease
 - IP-CIDR,45.254.48.1/32,Netease
 - IP-CIDR,47.100.127.239/32,Netease
 - IP-CIDR,59.111.160.195/32,Netease
 - IP-CIDR,59.111.160.197/32,Netease
 - IP-CIDR,59.111.181.35/32,Netease
 - IP-CIDR,59.111.181.38/32,Netease
 - IP-CIDR,59.111.181.60/32,Netease
 - IP-CIDR,101.71.154.241/32,Netease
 - IP-CIDR,103.126.92.132/32,Netease
 - IP-CIDR,103.126.92.133/32,Netease
 - IP-CIDR,112.13.119.17/32,Netease
 - IP-CIDR,112.13.122.1/32,Netease
 - IP-CIDR,115.236.118.33/32,Netease
 - IP-CIDR,115.236.121.1/32,Netease
 - IP-CIDR,118.24.63.156/32,Netease
 - IP-CIDR,193.112.159.225/32,Netease
 - IP-CIDR,223.252.199.66/32,Netease
 - IP-CIDR,223.252.199.67/32,Netease
 - DOMAIN-SUFFIX,aaplimg.com,Apple
 - DOMAIN-SUFFIX,apple.co,Apple
 - DOMAIN-SUFFIX,apple.com,Apple
 - DOMAIN-SUFFIX,apple.com.cn,Apple
 - DOMAIN-SUFFIX,apple-cloudkit.com,Apple
 - DOMAIN-SUFFIX,apple-livephotoskit.com,Apple
 - DOMAIN-SUFFIX,apple-mapkit.com,Apple
 - DOMAIN-SUFFIX,applemusic.com,Apple
 - DOMAIN-SUFFIX,appstore.com,Apple
 - DOMAIN-SUFFIX,apzones.com,Apple
 - DOMAIN-SUFFIX,cdn-apple.com,Apple
 - DOMAIN-SUFFIX,icloud.com,Apple
 - DOMAIN-SUFFIX,icloud.com.cn,Apple
 - DOMAIN-SUFFIX,icloud-content.com,Apple
 - DOMAIN-SUFFIX,me.com,Apple
 - DOMAIN-SUFFIX,mzstatic.com,Apple
 - DOMAIN-KEYWORD,apple.com.akadns.net,Apple
 - DOMAIN-KEYWORD,apple.com.edgekey.net,Apple
 - DOMAIN-KEYWORD,apple-support.akadns.net,Apple
 - DOMAIN-KEYWORD,icloud.com.akadns.net,Apple
 - DOMAIN-SUFFIX,9cache.com,Proxies
 - DOMAIN-SUFFIX,9gag.com,Proxies
 - DOMAIN-SUFFIX,abc.com,Proxies
 - DOMAIN-SUFFIX,anchor.fm,Proxies
 - DOMAIN-SUFFIX,archive.fo,Proxies
 - DOMAIN-SUFFIX,archive.org,Proxies
 - DOMAIN-SUFFIX,archive.ph,Proxies
 - DOMAIN-SUFFIX,archiveofourown.org,Proxies
 - DOMAIN-SUFFIX,artstation.com,Proxies
 - DOMAIN-SUFFIX,ask.com,Proxies
 - DOMAIN-SUFFIX,avg.com,Proxies
 - DOMAIN-SUFFIX,axios.com,Proxies
 - DOMAIN-SUFFIX,bandcamp.com,Proxies
 - DOMAIN-SUFFIX,bandwagonhost.com,Proxies
 - DOMAIN-SUFFIX,bbc.com,Proxies
 - DOMAIN-SUFFIX,behance.net,Proxies
 - DOMAIN-SUFFIX,bit.ly,Proxies
 - DOMAIN-SUFFIX,bloglovin.com,Proxies
 - DOMAIN-SUFFIX,blubrry.com,Proxies
 - DOMAIN-SUFFIX,box.com,Proxies
 - DOMAIN-SUFFIX,brave.com,Proxies
 - DOMAIN-SUFFIX,bullguard.com,Proxies
 - DOMAIN-SUFFIX,castbox.fm,Proxies
 - DOMAIN-SUFFIX,change.org,Proxies
 - DOMAIN-SUFFIX,cloudcone.com,Proxies
 - DOMAIN-SUFFIX,clyp.it,Proxies
 - DOMAIN-SUFFIX,cna.com.tw,Proxies
 - DOMAIN-SUFFIX,conoha.jp,Proxies
 - DOMAIN-SUFFIX,coursehero.com,Proxies
 - DOMAIN-SUFFIX,c-span.org,Proxies
 - DOMAIN-SUFFIX,dailymotion.com,Proxies
 - DOMAIN-SUFFIX,daum.net,Proxies
 - DOMAIN-SUFFIX,deadline.com,Proxies
 - DOMAIN-SUFFIX,depositphotos.com,Proxies
 - DOMAIN-SUFFIX,deviantart.com,Proxies
 - DOMAIN-SUFFIX,deviantart.net,Proxies
 - DOMAIN-SUFFIX,disconnect.me,Proxies
 - DOMAIN-SUFFIX,disqus.com,Proxies
 - DOMAIN-SUFFIX,dlive.tv,Proxies
 - DOMAIN-SUFFIX,dowjones.com,Proxies
 - DOMAIN-SUFFIX,duckduckgo.com,Proxies
 - DOMAIN-SUFFIX,earthcam.com,Proxies
 - DOMAIN-SUFFIX,edx-cdn.org,Proxies
 - DOMAIN-SUFFIX,encyclopedia.com,Proxies
 - DOMAIN-SUFFIX,feeder.co,Proxies
 - DOMAIN-SUFFIX,feedly.com,Proxies
 - DOMAIN-SUFFIX,flickr.com,Proxies
 - DOMAIN-SUFFIX,flipboard.com,Proxies
 - DOMAIN-SUFFIX,flitto.com,Proxies
 - DOMAIN-SUFFIX,foreignaffairs.com,Proxies
 - DOMAIN-SUFFIX,foreignpolicy.com,Proxies
 - DOMAIN-SUFFIX,ft.com,Proxies
 - DOMAIN-SUFFIX,ftchinese.com,Proxies
 - DOMAIN-SUFFIX,ftimg.net,Proxies
 - DOMAIN-SUFFIX,genius.com,Proxies
 - DOMAIN-SUFFIX,getsync.com,Proxies
 - DOMAIN-SUFFIX,gfw.report,Proxies
 - DOMAIN-SUFFIX,git.io,Proxies
 - DOMAIN-SUFFIX,githack.com,Proxies
 - DOMAIN-SUFFIX,graphql.org,Proxies
 - DOMAIN-SUFFIX,hackmd.io,Proxies
 - DOMAIN-SUFFIX,heroku.com,Proxies
 - DOMAIN-SUFFIX,hket.com,Proxies
 - DOMAIN-SUFFIX,huffpost.com,Proxies
 - DOMAIN-SUFFIX,i-cable.com,Proxies
 - DOMAIN-SUFFIX,imgur.com,Proxies
 - DOMAIN-SUFFIX,independent.co.uk,Proxies
 - DOMAIN-SUFFIX,inoreader.com,Proxies
 - DOMAIN-SUFFIX,is.gd,Proxies
 - DOMAIN-SUFFIX,issuu.com,Proxies
 - DOMAIN-SUFFIX,istockphoto.com,Proxies
 - DOMAIN-SUFFIX,justpaste.it,Proxies
 - DOMAIN-SUFFIX,kakao.com,Proxies
 - DOMAIN-SUFFIX,kobo.com,Proxies
 - DOMAIN-SUFFIX,listennotes.com,Proxies
 - DOMAIN-SUFFIX,livestream.com,Proxies
 - DOMAIN-SUFFIX,mailchimp.com,Proxies
 - DOMAIN-SUFFIX,matrix.org,Proxies
 - DOMAIN-SUFFIX,medibang.com,Proxies
 - DOMAIN-SUFFIX,medium.com,Proxies
 - DOMAIN-SUFFIX,mega.co.nz,Proxies
 - DOMAIN-SUFFIX,mega.io,Proxies
 - DOMAIN-SUFFIX,mega.nz,Proxies
 - DOMAIN-SUFFIX,mixlr.com,Proxies
 - DOMAIN-SUFFIX,moon.fm,Proxies
 - DOMAIN-SUFFIX,mubi.com,Proxies
 - DOMAIN-SUFFIX,myspace.com,Proxies
 - DOMAIN-SUFFIX,myspacecdn.com,Proxies
 - DOMAIN-SUFFIX,nbcnews.com,Proxies
 - DOMAIN-SUFFIX,neowin.net,Proxies
 - DOMAIN-SUFFIX,newstatesman.com,Proxies
 - DOMAIN-SUFFIX,newsweek.com,Proxies
 - DOMAIN-SUFFIX,newyorker.com,Proxies
 - DOMAIN-SUFFIX,now.com,Proxies
 - DOMAIN-SUFFIX,ok.ru,Proxies
 - DOMAIN-SUFFIX,omny.fm,Proxies
 - DOMAIN-SUFFIX,openvpn.net,Proxies
 - DOMAIN-SUFFIX,owltail.com,Proxies
 - DOMAIN-SUFFIX,oxfordscholarship.com,Proxies
 - DOMAIN-SUFFIX,parsevideo.com,Proxies
 - DOMAIN-SUFFIX,paste.ee,Proxies
 - DOMAIN-SUFFIX,pastie.org,Proxies
 - DOMAIN-SUFFIX,pcloud.com,Proxies
 - DOMAIN-SUFFIX,peing.net,Proxies
 - DOMAIN-SUFFIX,player.fm,Proxies
 - DOMAIN-SUFFIX,podbean.com,Proxies
 - DOMAIN-SUFFIX,prism-break.org,Proxies
 - DOMAIN-SUFFIX,privoxy.org,Proxies
 - DOMAIN-SUFFIX,proxifier.com,Proxies
 - DOMAIN-SUFFIX,quora.com,Proxies
 - DOMAIN-SUFFIX,quoracdn.net,Proxies
 - DOMAIN-SUFFIX,qz.com,Proxies
 - DOMAIN-SUFFIX,radioline.co,Proxies
 - DOMAIN-SUFFIX,reabble.com,Proxies
 - DOMAIN-SUFFIX,redditlist.com,Proxies
 - DOMAIN-SUFFIX,resilio.com,Proxies
 - DOMAIN-SUFFIX,rsshub.app,Proxies
 - DOMAIN-SUFFIX,rthk.hk,Proxies
 - DOMAIN-SUFFIX,scmp.com,Proxies
 - DOMAIN-SUFFIX,scribd.com,Proxies
 - DOMAIN-SUFFIX,search.com,Proxies
 - DOMAIN-SUFFIX,shutterstock.com,Proxies
 - DOMAIN-SUFFIX,signal.org,Proxies
 - DOMAIN-SUFFIX,sketchappsources.com,Proxies
 - DOMAIN-SUFFIX,slideshare.net,Proxies
 - DOMAIN-SUFFIX,smartmailcloud.com,Proxies
 - DOMAIN-SUFFIX,smh.com.au,Proxies
 - DOMAIN-SUFFIX,speakerdeck.com,Proxies
 - DOMAIN-SUFFIX,spideroak.com,Proxies
 - DOMAIN-SUFFIX,spiegel.de,Proxies
 - DOMAIN-SUFFIX,startpage.com,Proxies
 - DOMAIN-SUFFIX,steemit.com,Proxies
 - DOMAIN-SUFFIX,straitstimes.com,Proxies
 - DOMAIN-SUFFIX,streamable.com,Proxies
 - DOMAIN-SUFFIX,substack.com,Proxies
 - DOMAIN-SUFFIX,swissinfo.ch,Proxies
 - DOMAIN-SUFFIX,tapatalk.com,Proxies
 - DOMAIN-SUFFIX,techspot.com,Proxies
 - DOMAIN-SUFFIX,textnow.me,Proxies
 - DOMAIN-SUFFIX,theage.com.au,Proxies
 - DOMAIN-SUFFIX,theatlantic.com,Proxies
 - DOMAIN-SUFFIX,theaustralian.com.au,Proxies
 - DOMAIN-SUFFIX,theconversation.com,Proxies
 - DOMAIN-SUFFIX,thediplomat.com,Proxies
 - DOMAIN-SUFFIX,theguardian.com,Proxies
 - DOMAIN-SUFFIX,theinitium.com,Proxies
 - DOMAIN-SUFFIX,themoviedb.org,Proxies
 - DOMAIN-SUFFIX,thetvdb.com,Proxies
 - DOMAIN-SUFFIX,time.com,Proxies
 - DOMAIN-SUFFIX,tineye.com,Proxies
 - DOMAIN-SUFFIX,tiny.cc,Proxies
 - DOMAIN-SUFFIX,torproject.org,Proxies
 - DOMAIN-SUFFIX,tradingview.com,Proxies
 - DOMAIN-SUFFIX,turbobit.net,Proxies
 - DOMAIN-SUFFIX,tutanota.com,Proxies
 - DOMAIN-SUFFIX,urbandictionary.com,Proxies
 - DOMAIN-SUFFIX,ustream.tv,Proxies
 - DOMAIN-SUFFIX,v2ex.com,Proxies
 - DOMAIN-SUFFIX,venturebeat.com,Proxies
 - DOMAIN-SUFFIX,viber.com,Proxies
 - DOMAIN-SUFFIX,vimeo.com,Proxies
 - DOMAIN-SUFFIX,voxer.com,Proxies
 - DOMAIN-SUFFIX,vzw.com,Proxies
 - DOMAIN-SUFFIX,washingtonpost.com,Proxies
 - DOMAIN-SUFFIX,wattpad.com,Proxies
 - DOMAIN-SUFFIX,welt.de,Proxies
 - DOMAIN-SUFFIX,whoer.net,Proxies
 - DOMAIN-SUFFIX,wikimapia.org,Proxies
 - DOMAIN-SUFFIX,wikiwand.com,Proxies
 - DOMAIN-SUFFIX,wire.com,Proxies
 - DOMAIN-SUFFIX,wireguard.com,Proxies
 - DOMAIN-SUFFIX,wn.com,Proxies
 - DOMAIN-SUFFIX,worldcat.org,Proxies
 - DOMAIN-SUFFIX,wsj.com,Proxies
 - DOMAIN-SUFFIX,wsj.net,Proxies
 - DOMAIN-SUFFIX,x.co,Proxies
 - DOMAIN-SUFFIX,yandex.ru,Proxies
 - DOMAIN-SUFFIX,you-get.org,Proxies
 - DOMAIN-SUFFIX,zaobao.com,Proxies
 - DOMAIN-SUFFIX,zello.com,Proxies
 - DOMAIN-SUFFIX,zeronet.io,Proxies
 - DOMAIN-SUFFIX,z-lib.org,Proxies
 - DOMAIN-SUFFIX,zophar.net,Proxies
 - DOMAIN-SUFFIX,zyxel.com,Proxies
 - DOMAIN,lab.skk.moe,Proxies
 - DOMAIN,ocsp.int-x3.letsencrypt.org,Proxies
 - DOMAIN,a248.e.akamai.net,Proxies
 - DOMAIN,a771.dscq.akamai.net,Proxies
 - DOMAIN-SUFFIX,amazon.co.jp,Proxies
 - DOMAIN,d3c33hcgiwev3.cloudfront.net,Proxies
 - DOMAIN,payments-jp.amazon.com,Proxies
 - DOMAIN,s3-ap-northeast-1.amazonaws.com,Proxies
 - DOMAIN,s3-ap-southeast-2.amazonaws.com,Proxies
 - DOMAIN-SUFFIX,abc.xyz,Proxies
 - DOMAIN-SUFFIX,admob.com,Proxies
 - DOMAIN-SUFFIX,adsense.com,Proxies
 - DOMAIN-SUFFIX,advertisercommunity.com,Proxies
 - DOMAIN-SUFFIX,ampproject.org,Proxies
 - DOMAIN-SUFFIX,android.com,Proxies
 - DOMAIN-SUFFIX,androidify.com,Proxies
 - DOMAIN-SUFFIX,androidtv.com,Proxies
 - DOMAIN-SUFFIX,api.ai,Proxies
 - DOMAIN-SUFFIX,apigee.com,Proxies
 - DOMAIN-SUFFIX,appspot.com,Proxies
 - DOMAIN-SUFFIX,blogblog.com,Proxies
 - DOMAIN-SUFFIX,blogger.com,Proxies
 - DOMAIN-SUFFIX,chrome.com,Proxies
 - DOMAIN-SUFFIX,chromium.org,Proxies
 - DOMAIN-SUFFIX,debug.com,Proxies
 - DOMAIN-SUFFIX,dialogflow.com,Proxies
 - DOMAIN-SUFFIX,feedburner.com,Proxies
 - DOMAIN-SUFFIX,firebaseio.com,Proxies
 - DOMAIN-SUFFIX,g.co,Proxies
 - DOMAIN-SUFFIX,getoutline.org,Proxies
 - DOMAIN-SUFFIX,ggpht.com,Proxies
 - DOMAIN-SUFFIX,gmail.com,Proxies
 - DOMAIN-SUFFIX,gmodules.com,Proxies
 - DOMAIN-SUFFIX,googleapis.cn,Proxies
 - DOMAIN-SUFFIX,gvt0.com,Proxies
 - DOMAIN-SUFFIX,gvt1.com,Proxies
 - DOMAIN-SUFFIX,gvt3.com,Proxies
 - DOMAIN-SUFFIX,itasoftware.com,Proxies
 - DOMAIN-SUFFIX,on2.com,Proxies
 - DOMAIN-SUFFIX,recaptcha.net,Proxies
 - DOMAIN-SUFFIX,schema.org,Proxies
 - DOMAIN-SUFFIX,tensorflow.org,Proxies
 - DOMAIN-SUFFIX,tfhub.dev,Proxies
 - DOMAIN-SUFFIX,tiltbrush.com,Proxies
 - DOMAIN-SUFFIX,waymo.com,Proxies
 - DOMAIN-SUFFIX,web.dev,Proxies
 - DOMAIN-SUFFIX,webmproject.org,Proxies
 - DOMAIN-SUFFIX,webrtc.org,Proxies
 - DOMAIN-SUFFIX,widevine.com,Proxies
 - DOMAIN-SUFFIX,xn--ngstr-lra8j.com,Proxies
 - DOMAIN-SUFFIX,zynamics.com,Proxies
 - DOMAIN-KEYWORD,google,Proxies
 - DOMAIN-KEYWORD,.blogspot.,Proxies
 - DOMAIN-SUFFIX,goog,Proxies
 - DOMAIN,testflight.apple.com,Proxies
 - DOMAIN-SUFFIX,gravatar.com,Proxies
 - DOMAIN-SUFFIX,tumblr.com,Proxies
 - DOMAIN-SUFFIX,videopress.com,Proxies
 - DOMAIN-SUFFIX,wordpress.com,Proxies
 - DOMAIN-SUFFIX,bloomberg.cn,Proxies
 - DOMAIN-SUFFIX,bloomberg.com,Proxies
 - DOMAIN-SUFFIX,bloomberg.de,Proxies
 - DOMAIN-SUFFIX,bloombergview.com,Proxies
 - DOMAIN-SUFFIX,clubhouseapi.com,Proxies
 - DOMAIN-SUFFIX,joinclubhouse.com,Proxies
 - DOMAIN,clubhouse.pubnubapi.com,Proxies
 - DOMAIN-SUFFIX,aex.com,Proxies
 - DOMAIN-SUFFIX,bibox.com,Proxies
 - DOMAIN-SUFFIX,binance.cc,Proxies
 - DOMAIN-SUFFIX,binance.com,Proxies
 - DOMAIN-SUFFIX,binance.us,Proxies
 - DOMAIN-SUFFIX,bitcointalk.org,Proxies
 - DOMAIN-SUFFIX,bitfinex.com,Proxies
 - DOMAIN-SUFFIX,bithumb.com,Proxies
 - DOMAIN-SUFFIX,bitmex.com,Proxies
 - DOMAIN-SUFFIX,bitstamp.net,Proxies
 - DOMAIN-SUFFIX,bittrex.com,Proxies
 - DOMAIN-SUFFIX,bybit.com,Proxies
 - DOMAIN-SUFFIX,coinbase.com,Proxies
 - DOMAIN-SUFFIX,coincheck.com,Proxies
 - DOMAIN-SUFFIX,coingecko.com,Proxies
 - DOMAIN-SUFFIX,coinmarketcap.com,Proxies
 - DOMAIN-SUFFIX,coinone.co.kr,Proxies
 - DOMAIN-SUFFIX,etherscan.io,Proxies
 - DOMAIN-SUFFIX,ftx.com,Proxies
 - DOMAIN-SUFFIX,gate.io,Proxies
 - DOMAIN-SUFFIX,gemini.com,Proxies
 - DOMAIN-SUFFIX,huobi.com,Proxies
 - DOMAIN-SUFFIX,korbit.co.kr,Proxies
 - DOMAIN-SUFFIX,kraken.com,Proxies
 - DOMAIN-SUFFIX,kucoin.com,Proxies
 - DOMAIN-SUFFIX,liquid.com,Proxies
 - DOMAIN-SUFFIX,okex.com,Proxies
 - DOMAIN-SUFFIX,okx.com,Proxies
 - DOMAIN-SUFFIX,poloniex.com,Proxies
 - DOMAIN-SUFFIX,sushi.com,Proxies
 - DOMAIN-SUFFIX,uniswap.org,Proxies
 - DOMAIN-SUFFIX,zb.com,Proxies
 - DOMAIN-SUFFIX,discord.com,Proxies
 - DOMAIN-SUFFIX,discordapp.com,Proxies
 - DOMAIN-SUFFIX,discordapp.net,Proxies
 - DOMAIN-SUFFIX,dropbox.com,Proxies
 - DOMAIN-SUFFIX,dropboxapi.com,Proxies
 - DOMAIN-SUFFIX,dropboxusercontent.com,Proxies
 - DOMAIN-SUFFIX,freetls.fastly.net,Proxies
 - DOMAIN,cloud-cdn-digitalocean-com.global.ssl.fastly.net,Proxies
 - DOMAIN,github.global.ssl.fastly.net,Proxies
 - DOMAIN,nytimes.map.fastly.net,Proxies
 - DOMAIN-SUFFIX,line.me,Proxies
 - DOMAIN-SUFFIX,line-apps.com,Proxies
 - DOMAIN-SUFFIX,line-scdn.net,Proxies
 - DOMAIN-SUFFIX,naver.jp,Proxies
 - IP-CIDR,103.2.30.0/23,Proxies,no-resolve
 - IP-CIDR,125.209.208.0/20,Proxies,no-resolve
 - IP-CIDR,147.92.128.0/17,Proxies,no-resolve
 - IP-CIDR,203.104.144.0/21,Proxies,no-resolve
 - DOMAIN-SUFFIX,accountkit.com,Proxies
 - DOMAIN-SUFFIX,cdninstagram.com,Proxies
 - DOMAIN-SUFFIX,f8.com,Proxies
 - DOMAIN-SUFFIX,facebookmail.com,Proxies
 - DOMAIN-SUFFIX,fb.com,Proxies
 - DOMAIN-SUFFIX,fb.me,Proxies
 - DOMAIN-SUFFIX,fb.watch,Proxies
 - DOMAIN-SUFFIX,fbaddins.com,Proxies
 - DOMAIN-SUFFIX,fbcdn.net,Proxies
 - DOMAIN-SUFFIX,fbsbx.com,Proxies
 - DOMAIN-SUFFIX,fbworkmail.com,Proxies
 - DOMAIN-SUFFIX,instagram.com,Proxies
 - DOMAIN-SUFFIX,m.me,Proxies
 - DOMAIN-SUFFIX,messenger.com,Proxies
 - DOMAIN-SUFFIX,oculus.com,Proxies
 - DOMAIN-SUFFIX,oculuscdn.com,Proxies
 - DOMAIN-SUFFIX,readyatdawn.com,Proxies
 - DOMAIN-SUFFIX,rocksdb.org,Proxies
 - DOMAIN-SUFFIX,whatsapp.com,Proxies
 - DOMAIN-SUFFIX,whatsapp.net,Proxies
 - DOMAIN-KEYWORD,.facebook.,Proxies
 - DOMAIN-SUFFIX,aka.ms,Proxies
 - DOMAIN-SUFFIX,github.blog,Proxies
 - DOMAIN-SUFFIX,github.com,Proxies
 - DOMAIN-SUFFIX,github.io,Proxies
 - DOMAIN-SUFFIX,githubusercontent.com,Proxies
 - DOMAIN-SUFFIX,onedrive.live.com,Proxies
 - DOMAIN-SUFFIX,streaming.mediaservices.windows.net,Proxies
 - DOMAIN,assets1.xboxlive.com,Proxies
 - DOMAIN,assets2.xboxlive.com,Proxies
 - DOMAIN,az416426.vo.msecnd.net,Proxies
 - DOMAIN,az668014.vo.msecnd.net,Proxies
 - DOMAIN-KEYWORD,.pinterest.,Proxies
 - DOMAIN-SUFFIX,pixiv.net,Proxies
 - DOMAIN-SUFFIX,pixiv.org,Proxies
 - DOMAIN-SUFFIX,pximg.net,Proxies
 - DOMAIN-SUFFIX,redd.it,Proxies
 - DOMAIN-SUFFIX,reddit.com,Proxies
 - DOMAIN-SUFFIX,redditmedia.com,Proxies
 - DOMAIN-SUFFIX,redditstatic.com,Proxies
 - DOMAIN-SUFFIX,reuters.com,Proxies
 - DOMAIN-SUFFIX,reutersmedia.net,Proxies
 - DOMAIN-SUFFIX,steamcommunity.com,Proxies
 - DOMAIN-SUFFIX,legra.ph,Proxies
 - DOMAIN-SUFFIX,t.me,Proxies
 - DOMAIN-SUFFIX,tdesktop.com,Proxies
 - DOMAIN-SUFFIX,telegra.ph,Proxies
 - DOMAIN-SUFFIX,telegram.me,Proxies
 - DOMAIN-SUFFIX,telegram.org,Proxies
 - DOMAIN-SUFFIX,telesco.pe,Proxies
 - IP-CIDR,91.108.4.0/22,Proxies,no-resolve
 - IP-CIDR,91.108.8.0/22,Proxies,no-resolve
 - IP-CIDR,91.108.12.0/22,Proxies,no-resolve
 - IP-CIDR,91.108.16.0/22,Proxies,no-resolve
 - IP-CIDR,91.108.20.0/22,Proxies,no-resolve
 - IP-CIDR,91.108.56.0/22,Proxies,no-resolve
 - IP-CIDR,91.105.192.0/23,Proxies,no-resolve
 - IP-CIDR,149.154.160.0/20,Proxies,no-resolve
 - IP-CIDR,185.76.151.0/24,Proxies,no-resolve
 - IP-CIDR6,2001:b28:f23d::/48,Proxies,no-resolve
 - IP-CIDR6,2001:b28:f23f::/48,Proxies,no-resolve
 - IP-CIDR6,2001:67c:4e8::/48,Proxies,no-resolve
 - IP-CIDR6,2001:b28:f23c::/48,Proxies,no-resolve
 - IP-CIDR6,2a0a:f280::/32,Proxies,no-resolve
 - DOMAIN-SUFFIX,economist.com,Proxies
 - DOMAIN-SUFFIX,static-economist.com,Proxies
 - DOMAIN-SUFFIX,newyorktimes.com,Proxies
 - DOMAIN-SUFFIX,nyt.com,Proxies
 - DOMAIN-SUFFIX,nytco.com,Proxies
 - DOMAIN-SUFFIX,nytimes.com,Proxies
 - DOMAIN-SUFFIX,nytimg.com,Proxies
 - DOMAIN-SUFFIX,nytlog.com,Proxies
 - DOMAIN-SUFFIX,nytstyle.com,Proxies
 - DOMAIN-SUFFIX,tmagazine.com,Proxies
 - DOMAIN-SUFFIX,periscope.tv,Proxies
 - DOMAIN-SUFFIX,pscp.tv,Proxies
 - DOMAIN-SUFFIX,t.co,Proxies
 - DOMAIN-SUFFIX,tweetdeck.com,Proxies
 - DOMAIN-SUFFIX,twimg.co,Proxies
 - DOMAIN-SUFFIX,twimg.com,Proxies
 - DOMAIN-SUFFIX,twitpic.com,Proxies
 - DOMAIN-SUFFIX,twitter.com,Proxies
 - DOMAIN-SUFFIX,twitter.jp,Proxies
 - DOMAIN-SUFFIX,vine.co,Proxies
 - DOMAIN-SUFFIX,mediawiki.org,Proxies
 - DOMAIN-SUFFIX,wikibooks.org,Proxies
 - DOMAIN-SUFFIX,wikidata.org,Proxies
 - DOMAIN-SUFFIX,wikileaks.org,Proxies
 - DOMAIN-SUFFIX,wikimedia.org,Proxies
 - DOMAIN-SUFFIX,wikimediafoundation.org,Proxies
 - DOMAIN-SUFFIX,wikinews.org,Proxies
 - DOMAIN-SUFFIX,wikipedia.org,Proxies
 - DOMAIN-SUFFIX,wikiquote.org,Proxies
 - DOMAIN-SUFFIX,wikisource.org,Proxies
 - DOMAIN-SUFFIX,wikiversity.org,Proxies
 - DOMAIN-SUFFIX,wikivoyage.org,Proxies
 - DOMAIN-SUFFIX,wiktionary.org,Proxies
 - DOMAIN-SUFFIX,yahoo.com,Proxies
 - DOMAIN,search.yahoo.co.jp,Proxies
 - DOMAIN-SUFFIX,yadi.sk,Proxies
 - DOMAIN,disk.yandex.com,Proxies
 - DOMAIN-SUFFIX,aicoin.com,Proxies
 - DOMAIN-SUFFIX,aimoon.com,Proxies
 - DOMAIN-SUFFIX,engadget.com,Proxies
 - DOMAIN-SUFFIX,ifixit.com,Proxies
 - DOMAIN-SUFFIX,terabox.com,Proxies
 - DOMAIN-SUFFIX,zaobao.com.sg,Proxies
 - DOMAIN,wego.here.com,Proxies
 - DOMAIN-SUFFIX,go.dev,Proxies
 - DOMAIN-SUFFIX,golang.org,Proxies
 - DOMAIN-SUFFIX,appsto.re // Apple URL Shortener,Proxies
 - DOMAIN-SUFFIX,smoot.apple.com // Spotlight,Proxies
 - DOMAIN,amp-api.podcasts.apple.com // Podcasts,Proxies
 - DOMAIN,beta.music.apple.com // Apple Music Web,Proxies
 - DOMAIN,books.itunes.apple.com // iBooks Store download,Proxies
 - DOMAIN,lookup-api.apple.com // Look Up,Proxies
 - DOMAIN,radio.itunes.apple.com // Apple Music Radio,Proxies
 - DOMAIN,apps.apple.com,Proxies
 - DOMAIN,books.apple.com,Proxies
 - DOMAIN,itunes.apple.com,Proxies
 - DOMAIN,tv.apple.com,Proxies
 - DOMAIN,gateway.icloud.com,Proxies
 - DOMAIN-SUFFIX,apple.news,Proxies
 - DOMAIN,news-assets.apple.com,Proxies
 - DOMAIN,news-client.apple.com,Proxies
 - DOMAIN,news-client-search.apple.com,Proxies
 - DOMAIN,news-edge.apple.com,Proxies
 - DOMAIN,news-events.apple.com,Proxies
 - DOMAIN,apple.comscoreresearch.com,Proxies
 - DOMAIN-SUFFIX,bing.com,Proxies
 - DOMAIN-SUFFIX,linkedin.com,Proxies
 - DOMAIN-SUFFIX,licdn.com,Proxies
 - DOMAIN-SUFFIX,msn.com,Proxies
 - DOMAIN-SUFFIX,skype.com,Proxies
 - DOMAIN-SUFFIX,flyert.com,DIRECT
 - DOMAIN-SUFFIX,gandi.net,DIRECT
 - DOMAIN-SUFFIX,cm.steampowered.com // Steam Connect Manager Servers,DIRECT
 - DOMAIN,api.steampowered.com,DIRECT
 - DOMAIN,download.jetbrains.com,DIRECT
 - DOMAIN,origin-a.akamaihd.net // Origin Download,DIRECT
 - DOMAIN,outlook.office365.com,DIRECT
 - DOMAIN,smtp-mail.outlook.com,DIRECT
 - DOMAIN,smtp.office365.com,DIRECT
 - DOMAIN-SUFFIX,dl.delivery.mp.microsoft.com,DIRECT
 - DOMAIN-SUFFIX,update.microsoft.com,DIRECT
 - DOMAIN-SUFFIX,windowsupdate.com,DIRECT
 - DOMAIN-SUFFIX,windowsupdate.microsoft.com,DIRECT
 - DOMAIN,download.microsoft.com,DIRECT
 - DOMAIN,wustat.windows.com,DIRECT
 - DOMAIN,ntservicepack.microsoft.com,DIRECT
 - DOMAIN-SUFFIX,paypal.com,DIRECT
 - DOMAIN-SUFFIX,paypal.me,DIRECT
 - DOMAIN-SUFFIX,paypal-mktg.com,DIRECT
 - DOMAIN-SUFFIX,paypalobjects.com,DIRECT
 - IP-CIDR,182.254.116.0/24,DIRECT,no-resolve
 - IP-CIDR,203.205.238.0/23,DIRECT,no-resolve
 - IP-CIDR,203.205.254.0/23,DIRECT,no-resolve
 - DOMAIN,ip.istatmenus.app,DIRECT
 - DOMAIN,sms.imagetasks.com,DIRECT
 - DOMAIN-SUFFIX,netspeedtestmaster.com,DIRECT
 - DOMAIN,speedtest.macpaw.com,DIRECT
 - DOMAIN-SUFFIX,acg.rip,DIRECT
 - DOMAIN-SUFFIX,animebytes.tv,DIRECT
 - DOMAIN-SUFFIX,awesome-hd.me,DIRECT
 - DOMAIN-SUFFIX,broadcasthe.net,DIRECT
 - DOMAIN-SUFFIX,chdbits.co,DIRECT
 - DOMAIN-SUFFIX,classix-unlimited.co.uk,DIRECT
 - DOMAIN-SUFFIX,comicat.org,DIRECT
 - DOMAIN-SUFFIX,empornium.me,DIRECT
 - DOMAIN-SUFFIX,gazellegames.net,DIRECT
 - DOMAIN-SUFFIX,hdbits.org,DIRECT
 - DOMAIN-SUFFIX,hdchina.org,DIRECT
 - DOMAIN-SUFFIX,hddolby.com,DIRECT
 - DOMAIN-SUFFIX,hdhome.org,DIRECT
 - DOMAIN-SUFFIX,hdsky.me,DIRECT
 - DOMAIN-SUFFIX,icetorrent.org,DIRECT
 - DOMAIN-SUFFIX,jpopsuki.eu,DIRECT
 - DOMAIN-SUFFIX,keepfrds.com,DIRECT
 - DOMAIN-SUFFIX,madsrevolution.net,DIRECT
 - DOMAIN-SUFFIX,morethan.tv,DIRECT
 - DOMAIN-SUFFIX,m-team.cc,DIRECT
 - DOMAIN-SUFFIX,myanonamouse.net,DIRECT
 - DOMAIN-SUFFIX,nanyangpt.com,DIRECT
 - DOMAIN-SUFFIX,ncore.cc,DIRECT
 - DOMAIN-SUFFIX,open.cd,DIRECT
 - DOMAIN-SUFFIX,ourbits.club,DIRECT
 - DOMAIN-SUFFIX,passthepopcorn.me,DIRECT
 - DOMAIN-SUFFIX,privatehd.to,DIRECT
 - DOMAIN-SUFFIX,pterclub.com,DIRECT
 - DOMAIN-SUFFIX,redacted.ch,DIRECT
 - DOMAIN-SUFFIX,springsunday.net,DIRECT
 - DOMAIN-SUFFIX,tjupt.org,DIRECT
 - DOMAIN-SUFFIX,totheglory.im,DIRECT
 - GEOIP,CN,DIRECT,no-resolve
 - DOMAIN-SUFFIX,local,DIRECT
 - IP-CIDR,192.168.0.0/16,DIRECT,no-resolve
 - IP-CIDR,10.0.0.0/8,DIRECT,no-resolve
 - IP-CIDR,172.16.0.0/12,DIRECT,no-resolve
 - IP-CIDR,127.0.0.0/8,DIRECT,no-resolve
 - IP-CIDR,100.64.0.0/10,DIRECT,no-resolve
 - IP-CIDR6,::1/128,DIRECT,no-resolve
 - IP-CIDR6,fc00::/7,DIRECT,no-resolve
 - IP-CIDR6,fe80::/10,DIRECT,no-resolve
 - IP-CIDR6,fd00::/8,DIRECT,no-resolve
 - GEOIP,CN,DIRECT
 - MATCH,Proxies
