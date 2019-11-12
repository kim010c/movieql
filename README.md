# movieql

GraphQL을 이용한 영화 API만들기

setup

yarn init

yarn graphql-yoga

yarn global add babel-cli 안되면
yarn global add babel-cli --ignore-engines

yarn add babel-cli babel-preset-env babel-preset-stage-3 --dev

schema.graphql 파일{
데이터베이스 스키마(schema)를 작성할 때의 경험을 SQL 쿼리 작성으로 비유한다면, gql 스키마를 작성할 때의 경험은 C, C++의 헤더파일 작성에 비유가 됩니다.

    오브젝트 타입 : Person
    필드 : id,name, age, gender
    스칼라 타입 : String, ID, Int 등
    느낌표(!) : 필수 값을 의미(non-nullable)
    대괄호([, ]) : 배열을 의미(array)

}
오퍼레이션 네임 쿼리{
쿼리는 매우 편리 합니다. 굳이 비유하자면 쿼리용 함수 입니다. 데이터베이스 에서의 프로시져(procedure) 개념과 유사하다고 생각하면 됩니다.
}

리졸버(resolver){
gql 쿼리에서는 각각의 필드마다 함수가 하나씩 존재 한다고 생각하면 됩니다. 이 함수는 다음 타입을 반환합니다. 이러한 각각의 함수를 리졸버(resolver)라고 합니다. 만약 필드가 스칼라 값(문자열이나 숫자와 같은 primitive 타입)인 경우에는 실행이 종료됩니다. 즉 더 이상의 연쇄적인 리졸버 호출이 일어나지 않습니다. 하지만 필드의 타입이 스칼라 타입이 아닌 우리가 정의한 타입이라면 해당 타입의 리졸버를 호출되게 됩니다.

}

#10 이후
yarn add node-fetch //윈도우 페치같은거
