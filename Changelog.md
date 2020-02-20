Time: 2017/12/26  
Version: v0.0.6    

$\color{#FF3030}{11111111111111}$  
    Access_rule module :
        fix : 'host' not ignore case
    
    Log module :
        add directive : 'size_limit'
    
    Api module :
        upload API module
        fix : failed to request api
    
    Anti_mal_crawler module :
        fix : mistakenly identified as crawler
        add directive : 'dict_state'
    
    Anti_cc module :
        fix : no log in CC protection period
        add directive : 'attacks' 
    
    Secrules module :
        add action : 'WARN'
        add action : 'AUDIT'
        add action : 'ALLOW_PHASE'
        add directive : 'system_rules_state'
        add directive : 'recommend' in rules
        add directive : 'add_resp_headers' in rules
        fix : 'meta' not work when action is 'DENY'
        change the order of system_rule and user_defined_rules
    
    Others :
       upload doc : 轻松玩转OpenWAF之ELK
       upload doc : 深入研究OpenWAF之nginx配置
       upload doc : 轻松玩转OpenWAF之安装篇
       upload donation
       support waf bypass
       fix : return 500, ngx.req.raw_header() not support HTTP/2
       create CODE_OF_CONDUCT.md
       create CONTRIBUTING.md
       update docker version to 0.0.6
    
    New Release : 0.0.6
    
Time: 2017/04/10  
Version: v0.0.5  
    1. Rules
        Delete 30 rules which severity is "low".
    2. fix
        Failed to install on Ubuntu: undefined symbol GeoIP_continent_by_id
    3. Update docker version to 0.0.5
    4. New Release - 0.0.5
    
Time: 2017/03/20  
Version: v0.0.4  
    1. New Module - twaf_anti_cc  
        Anti http flood  
    2. Performance optimization
        optimaize RESPONSE_BODY variable to reduce memory
    3. add QQ group
        QQ group: 579790127
    4. fix
        4.1 loading error -- wrong comment
        4.2 return 500 response code -- string.char not support GBK
    5. Update docker version
    6. New Release - 0.0.4
    
Time: 2017/01/03  
Version: v0.0.3.170103_beta  
    1. New Module - twaf_anti_mal_crawler  
        Distinguish malicious crawler and some scan tools 
    
Time: 2016/12/05  
Version: v0.0.2.161205_beta  
    1. New Module - twaf_attack_response  
        Return custom response page When the request is rejected by OpenWAF  
    2. Api - api/stat[/policy_uuid]  
        Show statistical infomation  
    
Time: 2016/12/05  
Version: v0.0.1.161130_beta  
    1. Docker  
        build OpenWAF with docker  
    
Time: 2016/12/05  
Version: v0.0.1.161012_beta  
    1. log module  
        Send tcp/udp log  
    2. reqstat module  
        Statistics of request infomation  
    3. access rule  
        Publish applications  
    4. rule engine  
        Access Control  
    
