## 1:N 양방향
- N쪽에 외래키 존재. 연관관계의 주인.
- 연관관계 주인 엔티티에 `@ManyToOne`, `@JoinColumn(name = "FK")`으로 매핑
- 반대쪽에는 `@OneToMany(mappedBy = "")`
