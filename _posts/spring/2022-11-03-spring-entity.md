---
title: "[Spring] Entity"
author: Jiwonss
categories: [Spring]
tags: [spring]
---

## Entity 작성

Entity

```java
@Entity
public class SpringTestEntity {

    @Id
    private Long id;

}
```

@Data

@NoArgsConstructor, @AllArgsConstructor, @RequiredArgsConstructor

@ToString, @EqualsAndHashCode, @Builder

@Entity, @Table

@Id, @GeneratedValue, @Column

@NotNull, @NotBlank, @NotEmpty

@OneToOne, @OneToMany, @ManyToOne, @ManyToMany

FetchType.EAGER, FetchType.LAZY

@JoinColumn
