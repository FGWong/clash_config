

clash meta cofigure file in yaml format.
with proxy-providers and rule-providers

refer: https://github.com/MetaCubeX/mihomo/blob/Meta/docs/config.yaml

config_rules.yml
clash 的默认订阅配置, proxies-provider 在raspi 上生成
 rule-providers 主要依赖 https://cdn.jsdelivr.net/gh/Loyalsoldier/
  git@github.com:Loyalsoldier/clash-rules.git
  https://github.com/Loyalsoldier/clash-rules/tree/release
  以及本项目补充 ./ruleset
      classical_direct.yaml  支持传统的 rule规则写法， 不经代理的项
      manual_direct.yaml  只包含 domain 的写法 不经代理的项

      classical_proxy.yaml  支持传统的 rule规则写法， 经代理的项
      manual_proxy.yaml  只包含 domain 的写法 经代理的项

config_raspi.black_rule.yml , 更节省vpn流量的配置
  gfw.yaml 为proxy.yaml 的子集



获取cloudflare的ip范围, 在ruleset/classic_direct.yaml 中设置直连
cf_op 等代理 使用了cf边缘节点，两个边缘节点被cf设置禁止直接连接，所以会有连不上的情况
wget "https://www.cloudflare.com/ips-v4"
wget "https://www.cloudflare.com/ips-v6"

