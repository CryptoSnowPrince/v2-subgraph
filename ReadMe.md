yarn global add @graphprotocol/graph-cli
graph init --product hosted-service cryptosnowprince/v2-subgraph
cd v2-subgraph
graph codegen && graph build
graph auth --product hosted-service ACESS_TOKEN
graph deploy --product hosted-service cryptosnowprince/v2-subgraph
Queries (HTTP):     https://api.thegraph.com/subgraphs/name/cryptosnowprince/v2-subgraph