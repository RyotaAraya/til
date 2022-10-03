# 背景
instrment3はcognitoでユーザ認証を行なっているが、userのidなどを取得できない。idを取得できない(emailなどは取得できる)とpageのURLなどにidを使用できない。(emailだと個人情報になり微妙)会員登録時のuser情報をDBに格納し、IDを取得したい。また、cognitoとは別でuser情報を格納しておくことが推奨されている。

# 目的
user情報をcognitoのユーザプールに登録時、DynamoDBにも登録する。

# 構成

cognito→lambda→DynamoDB


# 参考

cognito→lambda



lambda→DynamoDB

https://k69blog.com/posts/how_to_insert_from_lambda_to_dynamodb/
