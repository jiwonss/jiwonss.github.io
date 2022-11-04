---
title: "[Spring] Annotation"
author: Jiwonss
categories: [Spring]
tags: [spring]
---

## Spring Framework

### Boot

|                                                              |
| ------------------------------------------------------------ |
| **@SpringBootApplication**                                   |
| org.springframework.boot.autoconfigure.SpringBootApplication |

### Beans

|                                                    |
| -------------------------------------------------- |
| **@Value**                                         |
| org.springframework.beans.factory.annotation.Value |

### Data

|                                                                  |
| ---------------------------------------------------------------- |
| **@CreatedDate**                                                 |
| org.springframework.data.annotation.CreatedDate                  |
| **@LastModifiedDate**                                            |
| org.springframework.data.annotation.LastModifiedDate             |
| **@EnableJpaAuditing**                                           |
| org.springframework.data.jpa.repository.config.EnableJpaAuditing |

### Stereotype

|                                           |
| ----------------------------------------- |
| **@Controller**                           |
| org.springframework.stereotype.Controller |
| **@Service**                              |
| org.springframework.stereotype.Service    |
| **@Repository**                           |
| org.springframework.stereotype.Repository |
| **@Component**                            |
| org.springframework.stereotype.Component  |

### Security

|                                                                                                |
| ---------------------------------------------------------------------------------------------- |
| **@EnableGlobalMethodSecurity**                                                                |
| org.springframework.security.config.annotation.method.configuration.EnableGlobalMethodSecurity |
| **@AuthenticationPrincipal**                                                                   |
| org.springframework.security.core.annotation.AuthenticationPrincipal                           |
| **@PreAuthorize**                                                                              |
| org.springframework.security.access.prepost.PreAuthorize                                       |
| **@EnableWebSecurity**                                                                         |
| org.springframework.security.config.annotation.web.configuration.EnableWebSecurity             |

### Transaction

|                                                          |
| -------------------------------------------------------- |
| **@Transactional**                                       |
| org.springframework.transaction.annotation.Transactional |

### Web

|                                                        |
| ------------------------------------------------------ |
| **@RestController**                                    |
| org.springframework.web.bind.annotation.RestController |
| **@RequestMapping**                                    |
| org.springframework.web.bind.annotation.RequestMapping |
| **@InitBinder**                                        |
| org.springframework.web.bind.annotation.InitBinder     |
| **@GetMapping**                                        |
| org.springframework.web.bind.annotation.GetMapping     |
| **@PostMapping**                                       |
| org.springframework.web.bind.annotation.PostMapping    |
| **@PutMapping**                                        |
| org.springframework.web.bind.annotation.PutMapping     |
| **@DeleteMapping**                                     |
| org.springframework.web.bind.annotation.DeleteMapping  |
| **@RequestParam**                                      |
| org.springframework.web.bind.annotation.RequestParam   |
| **@PathVariable**                                      |
| org.springframework.web.bind.annotation.PathVariable   |
| **@RequestBody**                                       |
| org.springframework.web.bind.annotation.RequestBody    |
| **@ModelAttribute**                                    |
| org.springframework.web.bind.annotation.ModelAttribute |

## Lombok

|                                |
| ------------------------------ |
| **@Data**                      |
| lombok.Data                    |
| **@NoArgsConstructor**         |
| lombok.NoArgsConstructor       |
| **@AllArgsConstructor**        |
| lombok.AllArgsConstructor      |
| **@RequiredArgsConstructor**   |
| lombok.RequiredArgsConstructor |
| **@ToString**                  |
| lombok.ToString                |
| **@EqualsAndHashCode**         |
| lombok.EqualsAndHashCode       |
| **@Builder**                   |
| lombok.Builder                 |
| **@Slf4j**                     |
| lombok.extern.slf4j.Slf4j      |

## Javax

### Persistence

|                                    |
| ---------------------------------- |
| **@Entity**                        |
| javax.persistence.Entity           |
| **@Table**                         |
| javax.persistence.Table            |
| **@Id**                            |
| javax.persistence.Id               |
| **@GeneratedValue**                |
| javax.persistence.GeneratedValue   |
| **@Column**                        |
| javax.persistence.Column           |
| **@OneToMany**                     |
| javax.persistence.OneToMany        |
| **@ManyToOne**                     |
| javax.persistence.ManyToOne        |
| **@JoinColumn**                    |
| javax.persistence.JoinColumn       |
| **@MappedSuperclass**              |
| javax.persistence.MappedSuperclass |
| **@EntityListeners**               |
| javax.persistence.EntityListeners  |

### Validation

|                                       |
| ------------------------------------- |
| **@Valid**                            |
| javax.validation.Valid                |
| **@NotNull**                          |
| javax.validation.constraints.NotNull  |
| **@NotBlank**                         |
| javax.validation.constraints.NotBlank |
| **@Email**                            |
| javax.validation.constraints.Email    |
| **@Pattern**                          |
| javax.validation.constraints.Pattern  |
