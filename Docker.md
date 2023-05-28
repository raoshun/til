# Dockerfile

## とくに理由がなければDockerfileは最上位に配置するのがよい
DockerfileのCOPYではローカルファイルをDockerfileからの相対パスで指定するが、Dockerfileより上位階層は参照できないという制約がある。そのためCOPYを用いる可能性があるDockerfileはリポジトリの最上位に置いておくのが無難。  
-- <cite>[Markdownでリンク付きで引用をするときの方法 – Tech Blog (techblg.app)](https://scrapbox.io/taka521-tech-notes/%E3%80%90Docker%E3%80%91COPY%E3%81%A7%E6%8C%87%E5%AE%9A%E3%81%95%E3%82%8C%E3%81%9F%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB%E3%81%AF%E3%80%81Dockerfile%E3%81%8C%E5%AD%98%E5%9C%A8%E3%81%99%E3%82%8B%E3%83%87%E3%82%A3%E3%83%AC%E3%82%AF%E3%83%88%E3%83%AA%E3%81%8B%E3%82%89%E3%81%AE%E7%9B%B8%E5%AF%BE%E3%83%91%E3%82%B9%E3%81%A7%E3%80%81%E8%A6%AA%E3%83%87%E3%82%A3%E3%83%AC%E3%82%AF%E3%83%88%E3%83%AA%E3%82%92%E8%A6%8B%E3%82%8C%E3%81%AA%E3%81%84)</cite>
