
clash meta cofigure file in yaml format.
with proxy-providers and rule-providers



config_rules.yml
clash 的默认订阅配置, proxies-provider 在raspi 上生成
 rule-providers 主要依赖 https://cdn.jsdelivr.net/gh/Loyalsoldier/
  git@github.com:Loyalsoldier/clash-rules.git
  https://github.com/Loyalsoldier/clash-rules/tree/release
  以及本项目补充 ./ruleset



config_raspi.black_rule.yml , 更节省vpn流量的配置
  gfw.yaml 为proxy.yaml 的子集
