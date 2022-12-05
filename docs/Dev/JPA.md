## N:1 양방향
- N쪽에 외래키 존재. 연관관계의 주인.
- 연관관계 주인 엔티티에 `@ManyToOne`, `@JoinColumn(name = "FK")`으로 매핑
- 반대쪽에는 `@OneToMany(mappedBy = "")`

## 1:1 양방향
- 더 자주 조회하는 쪽에 FK 넣기. 연관관계의 주인.
- 연관관계 주인 엔티티에 `@OneToOne, @JoinColumn(name = "FK")`
- 반대쪽에 `@OneToOne(mappedBy = "")`

## N:M 양방향
- 1:N, N:1로 풀어내기