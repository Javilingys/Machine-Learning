# [SOURCE (ORIGIN)](https://github.com/jonkrohn/ML-foundations)

# Content:
* [1. Data Structures for Linear Algebra](#data-structures-la)
    * [1.1. What Linear Algebra Is?](#what-is-la)
    * [1.2. Linear Algebra Execise](#la-exercise1)
    * [1.3. Tensors](#tensors)
    * [1.4. Scalars](#scalars)
    * [1.5. Vectors and Vector Transposition](#vectors)
    * [1.6. Norms and Unit Vectors](#norms)
    * [1.7. Basic, Orthogonal, and Orthonormal Vectors](#orthogonal)
    * [1.8. Matrix Tensors](#matrix)
    * [1.9. Generic Tensor Notation](#generic_notation)
    * [1.10. Exercise](#ex_section1)
* [2. Tensor Operations](#tensor_operations)
    * [2.1. Tensor Transponation](#transponation)
    * [2.2. Basic Tensor Arithmetic, incl. the Hadamard Product](#basic_arithmetic)
    * [2.3. Tensor Reduction](#reduction)
    * [2.4. The Dot Product](#dot_product)
    * [2.5. Exercises on Tensor Operations](#ex_section2)
    * [2.6. Solving Linear Systems with Substitution](#solve_subs)
    * [2.7. Solving Linear Systems with Elimination](#solve_elim)
* [3. Matrix Properties](#matrix_props)
    * [3.1. The Frobenius Norm](#frobenius)
    * [3.2. Matrix Multiplication](#matrix_mult)
    * [3.3. Symmetric and Identity Matrices](#sym_identity_matrix)
    * [3.4. Matrix Multiplication Exercises](#matrix_mult_ex)
    * [3.5. Matrix Inversion](#matrix_invesrion)
    * [3.6. Diagonal Matrices](#diagonal_m)
    * [3.7. Orthogonal Matrices](#orthogonal_matrix)
    * [3.8. Orthogonal Matrix Exercises](#orthogonal_matrix_ex)


# 1.	Data Structures for Linear Algebra <a name="data-structures-la"></a>
## 1.1.	What Linear Algebra Is? <a name="what-is-la"></a>

![pic1](https://sun9-east.userapi.com/sun9-17/s/v1/if2/3Jo2ycxHAcNA4MW3rvgcPpk3ytBVpH8S7sIbB7Yc3RYss1GKuuGsR_Av1hRNw1_f9smvBbVoSMrzaZuigtgnX7KV.jpg?size=1651x858&quality=96&type=album "pic1")
![pic2](https://sun9-west.userapi.com/sun9-68/s/v1/if2/F7J9ppEE3uptaI-_RHTu5WLy-0zwsHVf3RIF9PRoXBsDzTOwK9wgzpooxx2BVoGIi5prGURMd-FbrvOM2h9rv4Ny.jpg?size=1675x1070&quality=96&type=album "pic2")
![pic2](https://sun9-east.userapi.com/sun9-34/s/v1/if2/PsWKgvJ_MQmqKMFiz0IK3ZskVYdGprzv6FUoxXjes2o3MijWvqbe9eomxxerZFQ5pf6_SKv4ckCRNMWS9BaTENce.jpg?size=1620x960&quality=96&type=album "pic2")
![pic2](https://sun9-north.userapi.com/sun9-81/s/v1/if2/6d67A9Dp2b59cgV66twYm78KSkc7pVAFisO5w9hT93hF9ReoVmMfLR0BQ6H1VEREwN1cXZMwXplNa_CxSwcYmMwU.jpg?size=1891x980&quality=96&type=album "pic2")
![pic2](https://sun9-east.userapi.com/sun9-44/s/v1/if2/838gs5xLbYR-BRU6-gvxRDIajSrPzRIZaxebnZ7-NqFgCAhkz7ye-lVL3PWhduZf0EFC8_eaqPCXlA8sINOpIJ8_.jpg?size=1782x1077&quality=96&type=album "pic2")
![pic2](https://sun9-north.userapi.com/sun9-80/s/v1/if2/96GQ4clDHPpMjymInan9tWj2l57hlZjcdKmaPjezPZTo-jD77VtX_fvUMw3aZv5v27nzD0_9X7OLrwPDaI1j1T3Z.jpg?size=1524x1036&quality=96&type=album "pic2")
![pic2](https://sun9-west.userapi.com/sun9-61/s/v1/if2/0y8yVix0CzpGCBnIeCCLg7Khfv9nAdbBcpFkPhaoZisdpPqB75FNP_rwfkOQYuR9GchxSSJcv8LE6biM9vXjh3db.jpg?size=1690x933&quality=96&type=album "pic2")

## 1.2. Linear Algebra Execise <a name="la-exercise1"></a>

!["pic"](https://sun4.userapi.com/sun4-17/s/v1/if2/SyIcH5J1WQJ9ehQbIbQWmBiqUvNhEqgQIcfH_OGqPQlhN7E8X5FUTrIZsx2MBT-ZWU3mNDtdQBRu6pk2UdYv2jep.jpg?size=2388x1792&quality=95&type=album "pic")

## STOP AND TRY TO SOLVE THIS PROBLEM BY YOURSELF! NEXT WILL BE A SOLUTION!

!["pic"](https://sun9-west.userapi.com/sun9-38/s/v1/if2/RwnGmktxEOj7SMhO1k58P4DPUXRLL_5mxavg0ZmJzeph0Tvw8RuCYW7ypI7Ga35ai1clR6MkvSDn4A_KPbD6OFga.jpg?size=2388x1792&quality=95&type=album "pic")
!["123"](https://sun9-east.userapi.com/sun9-74/s/v1/if2/9xFchDgRqP0hzAvJMFQHwbTwJjmY2Oe-0xcC8tX9I4v07ixYeNUw_wiLHTLfSgdzoK81yz_9SULJAuSpnBDvy-Bu.jpg?size=1344x1792&quality=95&type=album "123")

## 1.3. Tensors <a name="tensors"></a>

!["123"](https://sun9-north.userapi.com/sun9-88/s/v1/if2/L1upchL4fE3p0HcGLWh0BsPP-lf5TI71VKgczaXeV_HE76UOEaF6xLTpYLeDfPZ0VBLR8yIgrf1NBr3G8c9aWI0-.jpg?size=2560x1263&quality=95&type=album "123")

## 1.4. Scalars <a name="scalars"></a>

!["123"](https://sun4.userapi.com/sun4-10/s/v1/if2/lCf2uyIPd1_nilziE0JqRk3Yw2LRHRdkdQnaBtpqrHY8j2w_Hk2OHJRZE7Ji_j-hha1bBOO97-5tWGbGrSk3TZOm.jpg?size=2560x1349&quality=95&type=album "123")

## 1.5. Vectors and Vector Transposition <a name="vectors"></a>

!["123"](https://sun9-east.userapi.com/sun9-24/s/v1/if2/EOWWYISx9nFYc0Mq4q6y20OW5Kcepm56eWTRcDk062HI7fgeECwKaW1OlV2NRq9xqkOVMjPSKniA-uj6Jeys7_qN.jpg?size=2560x1491&quality=95&type=album "123")
!["123"](https://sun9-west.userapi.com/sun9-38/s/v1/if2/KikkrFANgTM1f-1qnjq1zj7-JDd3131MXN7H4usM3LL4iNdpma30LeYDHWttC1gkkFp60FYb8K6S68uVTe36wdil.jpg?size=2560x1335&quality=95&type=album "123")

## 1.6. Norms and Unit Vectors <a name="norms"></a>

!["123"](https://sun9-west.userapi.com/sun9-11/s/v1/if2/l8gZBG20fKAEPHk20seG5LRcxfVXSR-2KA4v6tHJU9NpGso4HLXkQiiJaA4qEkM5nl_2dk4mSysXQw8W7Eia82KF.jpg?size=2560x1252&quality=95&type=album "123")
!["123"](https://sun9-west.userapi.com/sun9-10/s/v1/if2/Lr-lAQ98cs2LeuHdpueUBKHzg23PUWqZJAiEbbpKKfBmn7JLCyW35579Q_xfuJ_Flovry4guHGPSo1jmWo01MT2X.jpg?size=2560x1401&quality=95&type=album "123")
!["123"](https://sun9-east.userapi.com/sun9-60/s/v1/if2/bZr091TxSeMhFSjDsL5p_vc7bY-yQYL4ZvNZpSqlHRvF2oirEY-vnQz_1zgfDQLa8lZgVSWIHPLgK35FeEWrMfoS.jpg?size=2560x1479&quality=95&type=album "123")
!["123"](https://sun4.userapi.com/sun4-11/s/v1/if2/cJFWFxb78ZfGT5eEHyyP__9g9L2OuPVtUF6Nm-pa9D-M0MQ5utoeRdzJrAn9vC5trIBOaaJOsE96Katy-mxsdH9H.jpg?size=2560x615&quality=95&type=album "123")
!["123"](https://sun9-west.userapi.com/sun9-54/s/v1/if2/JOsKJZv3IHfOIqbnXr3KsK1AxkBmEexee5oJ4qIyFYC_uKRIUujR2kZ5-vKLecUaMl1NSgEq_Z215Nt74bG85i0V.jpg?size=2560x1099&quality=95&type=album "123")
!["123"](https://sun9-west.userapi.com/sun9-66/s/v1/if2/hD1dGFx-lRUQLGLnGzAGaPa8vu4CO-g6AVAwMOPRh6wBXIrmaWdLl9igDM2BE5WTC-qMb6MPQBf55tuXAVv7xueI.jpg?size=2560x1278&quality=95&type=album "123")
!["123"](https://sun9-west.userapi.com/sun9-12/s/v1/if2/PsTTixLrtG7Vf41fUc-Wc4-X4Phq6uD7GNn40PINQ5OG9XVlG_pdp4-sQ9e8SMzLAPeZXQXbxu3R40D9i_PGC2V6.jpg?size=2560x1092&quality=95&type=album "123")
!["123"](https://sun9-west.userapi.com/sun9-37/s/v1/if2/fWnSou4ow7M5h_6craXwX_Gb2GG52INppQvUMr1aGwfFR4hLUnnWsvXz73JHd9plB2Vakdw7znFP5Azk_1-Yfebw.jpg?size=2560x1383&quality=95&type=album "123")

## 1.7. Basic, Orthogonal, and Orthonormal Vectors <a name="orthogonal"></a>

!["123"](https://sun9-east.userapi.com/sun9-29/s/v1/if2/e47RdljOwnwzxDQ2TO-Vu2man8iDZgQAX5JBrvkYVjas0udIvs3vsv9VeRLaaFMyJGmVs1WviCn9plS_ylgpc5de.jpg?size=2560x1427&quality=95&type=album "123")
!["123"](https://sun9-west.userapi.com/sun9-45/s/v1/if2/j42qHw7r7PgDKLb8MSmh9uCeWi98XatsGPKBYetKD3qroVJ_Y3juqWEUviZNIOqj9airTJNj8mU96FbRXK8ZMO-r.jpg?size=2560x1439&quality=95&type=album "123")

## 1.8. Matrix Tensors <a name="matrix"></a>

!["123"](https://sun4.userapi.com/sun4-17/s/v1/if2/w-iSmGOCMdOzDWRZjxP9VW1D6jQ5lFeQqZP8fPqjtyVuBhbp9Y3wkDPaXxlUcx7_ss_9DxKVBGJG3VkyiLpITH6d.jpg?size=2560x1371&quality=95&type=album "123")

## 1.9. Generic Tensor Notation <a name="generic_notation"></a>

!["123"](https://sun9-north.userapi.com/sun9-88/s/v1/if2/LSbV93M8Yn2wDP2Yj1s6mGA7DZwWw2OOX-0dM5yiM68kfx7l9dfjRyH7LAg64VZeipSzEL9XfjG0bzKv0-CXmO3A.jpg?size=2560x594&quality=95&type=album "123")

## 1.10. Exercise <a name="ex_section1"></a>

!["123"](https://sun9-west.userapi.com/sun9-10/s/v1/if2/xTytYEmszf1w8ygONCbS0fy0yCxekmOmMnQcbY8ugTq33sbLtSRyx8EG06LIXcH_8ppfMo962Yle1GUsE87IyN3s.jpg?size=2560x1480&quality=95&type=album "123")
!["123"](https://sun9-north.userapi.com/sun9-85/s/v1/if2/P_AHv78ZFSxFGE8t2tIYllXxpsc79tJgeJdcya1VUFRApsaXCY9ZSA5cbQvuGERfhRUbN34WE8AH6B8yBZia5YFW.jpg?size=2228x1792&quality=95&type=album "123")

# 2.	Tensor Operations <a name="tensor_operations"></a>
## 2.1.	Tensor Transponation <a name="transponation"></a>

!["123"](https://sun9-west.userapi.com/sun9-1/s/v1/if2/NBZ2lGxXAcJyQw6Nr9mx242N87qg_taK8a4a_-Z2lA_CSGB_PAhQcAGpd7ns8Xw23ysKnrQDSXgSYOtQBTl2c-tP.jpg?size=2560x1412&quality=95&type=album "123")

## 2.2. Basic Tensor Arithmetic, incl. the Hadamard Product <a name="basic_arithmetic"></a>

!["123"](https://sun9-west.userapi.com/sun9-39/s/v1/if2/_Q71P9VadoTrdqoIx8m6VGKooVjDse3DKuW7DUCFG06jmTUg9Xjl_zQ9fh_zS1AF29OJ447HQPWfGt43bMcrbjAv.jpg?size=243x115&quality=96&type=album "123")
!["123"](https://sun9-east.userapi.com/sun9-20/s/v1/if2/hxd5pzLQigy_6rP6OVYD35so2-GAT3qNQRzMB9B5zY51se2nOWWeHwdIoeC5rpC2EyecPbMWibeI4yMv-D7M_0R-.jpg?size=1063x751&quality=96&type=album "123")
!["123"](https://sun9-north.userapi.com/sun9-77/s/v1/if2/Szh7lF-ZLQSUqG6RyVFh6fkFxTzlDOIkKQRwxePJal7ijH0BeUzJtqrNWbf9ibwcsuttHT2pvShN8jH9mkA5wRkR.jpg?size=907x346&quality=96&type=album "123")
!["123"](https://sun9-west.userapi.com/sun9-52/s/v1/if2/kB-3qubRUDEXxuOUb0xyz6tdVaE85lN3RIJjNTh_YOwThqanau4uTAXg8HyOLEvKTeHht7s6AObjsh8ifhSKFBwk.jpg?size=1718x230&quality=96&type=album "123")
!["123"](https://sun9-north.userapi.com/sun9-84/s/v1/if2/rBlnMJpKBDS-5SVmihbbqmw8yXGOfGYkBThvUdHCXQyzd4-PJnvNY7UkozMiHm7iF2dKCbvKWCBa9mtI613Cogo8.jpg?size=421x628&quality=96&type=album "123")
!["123"](https://sun9-east.userapi.com/sun9-35/s/v1/if2/5nShEd6lKdJLr6EnkCZalRd68P5IBbtUICJNzqzMmgWoES07N9aJJOJoTWFLyeL0qgRtnVBp7-OXXm8ZbLee4-kc.jpg?size=647x785&quality=96&type=album "123")

## 2.3. Tensor Reduction <a name="reduction"></a>

!["123"](https://sun9-east.userapi.com/sun9-20/s/v1/if2/YOWMpHY_tbxQ2DHn9iv9Pke32Xgu6-gDLGzKddXyPb8FpIMJbvhjj-K81cbRQeHdkWcH-fnqapxntvfR14gKriIO.jpg?size=1711x404&quality=96&type=album "123")
!["123"](https://sun9-west.userapi.com/sun9-50/s/v1/if2/WvvUsjyAGqg8PXsHCf7fHORKqeYw0ZDpoEZGKfEnTB_8T1jG6YNlpCnTVesGwg7OWPmM6F2VVMn8nlvIuJWXhnnE.jpg?size=557x476&quality=96&type=album "123")
!["123"](https://sun9-east.userapi.com/sun9-22/s/v1/if2/z-hnkIwfOkOtGsEqkhzvTvVF5mWx5QHLWGhvsgytq_kAW6IzzgEEw4BRKUQLh2uk2WU8MUhFrcemH9v6OggIAUk8.jpg?size=1307x695&quality=96&type=album "123")

## 2.4. The Dot Product <a name="dot_product"></a>

!["123"](https://sun9-west.userapi.com/sun9-11/s/v1/if2/Cg747HrQqAkM4HT21cOaiC4b9rn098lskyjGhsvqb0gMpGrWRJqHg2xPsBvP-86rFCzl6FZsev54ULY04E0KAG5v.jpg?size=1390x774&quality=96&type=album "123")
!["123"](https://sun9-north.userapi.com/sun9-80/s/v1/if2/XXZ48kN8mcJzwzDLUL98mawcQMeX4cKVTsDm0JJFB9gMJHo8uavC2pXS1yXQptnNfznQcTiDuirAg_cWECdjtN8M.jpg?size=900x709&quality=96&type=album "123")

## 2.5. Exercises on Tensor Operations <a name="ex_section2"></a>

!["123"](https://sun9-east.userapi.com/sun9-58/s/v1/if2/u0hglzKvh-ZH8cl2KI0X9CFirCUhYNbtX84tW8uswL71LcDL1hNoqarqzHCSkaAkeQJ6z6HP-qKw1jM0Ez_1pXyz.jpg?size=2560x1694&quality=95&type=album "123")
!["123"](https://sun9-west.userapi.com/sun9-66/s/v1/if2/T64CMtYYf55YkMyRY3Mtz7D5sfQsWHSL8OLRtP0g4W4lfjaI8JzzCeR4OB852pi6Ejg3f_YWkI3mcl-QLNuEcpNx.jpg?size=2560x1349&quality=95&type=album "123")

## 2.6. Solving Linear Systems with Substitution <a name="solve_subs"></a>

!["123"](https://sun9-west.userapi.com/sun9-40/s/v1/if2/PJF3PUIPObKxQrGtOaou6h8ZWYWgXNuKZILf8bqMv1ylRzHCkbXbM_JMUtNN3l_zpRAv0dqQTyjDBePnqw6Quiya.jpg?size=2560x1083&quality=95&type=album "123")
!["123"](https://sun9-east.userapi.com/sun9-36/s/v1/if2/rq785Cc5A971t-W1FQnGRVtKzV92fnEl6v1yUOEg30cFXx_3ZqdS_NzHrsEtPu6gHOsP7W8NYTcQ-zT8GOhCgTUQ.jpg?size=2304x1792&quality=95&type=album "123")
!["123"](https://sun9-west.userapi.com/sun9-48/s/v1/if2/cF_1cigB9_eeOu_7i0Md6xLSa5WjlrXIKoi3Ir29R88iEc1J4rcMzLId_Tx7AMrceReofMtoMqzOu2HgGO_fvlZG.jpg?size=2560x1362&quality=95&type=album "123")
!["123"](https://sun9-west.userapi.com/sun9-65/s/v1/if2/pajAMuLhSWnLbljJspgpAfjurFw49rHJ3G9oT6cnL6FMgbLhIS0roKt5cxSFw6eo8B-iT3YjqqRFCG_Bf0g83wK7.jpg?size=2118x1686&quality=95&type=album "123")
!["123"](https://sun9-west.userapi.com/sun9-51/s/v1/if2/VUPnsSFLMeBZAjMNBlrQHw1YXLAl9q-6zmnZ4c-9rvy-dZRfMcNdBKQB_buF6b8-gei87Lls4Q4-8gnG4WJ53-U9.jpg?size=2554x1792&quality=95&type=album "123")
!["123"](https://sun9-east.userapi.com/sun9-19/s/v1/if2/uifKVRC_cKpCoyut1sg1U0yN7Om-JgCFw0PlxjIE94OE-C7OcZqO02n2jhsIXq7APGNHbP8wnSKCRjkwXGp-DJFu.jpg?size=2272x1792&quality=95&type=album "123")
!["123"](https://sun9-west.userapi.com/sun9-56/s/v1/if2/KoDXdtJJOuO234bXeSu3rGtAvOhJ2CmIMvx141V6YWH7bFmBc29cbSHERXT8FU_tEk4a7as4soBjtxFSBafD177z.jpg?size=1436x1792&quality=95&type=album "123")

## 2.7. Solving Linear Systems with Elimination <a name="solve_elim"></a>

!["123"](https://sun9-east.userapi.com/sun9-58/s/v1/if2/qXh4JpALcIl_9z-LAPz3Ns782VqQ4NZ7oWjEb3tQnbV19bavuPJl3MHw2IAxN8o6qJVGXK0Ro4A3UutyzuSO1xBQ.jpg?size=2560x1354&quality=95&type=album "123")
!["123"](https://sun9-east.userapi.com/sun9-73/s/v1/if2/90DOUCL3I2phX95uP0z4wDzs4HRsSPKLXnw-FqT3u7NnOZLg7Ktds8Xaure2nCmyPB8vybo3lMRfcZcRVneCh7jt.jpg?size=2388x1790&quality=95&type=album "123")
!["123"](https://sun9-north.userapi.com/sun9-77/s/v1/if2/0xn5Yia_16KCbomICQOFZcypuct70jUVALLHaII0tkMIBU26EkAVl4IMtpwMx6Fh_IoRF1O0t8TfbEwIVAXQ2TLF.jpg?size=2560x1377&quality=95&type=album "123")
!["123"](https://sun9-west.userapi.com/sun9-63/s/v1/if2/2CHoIFhtR3fihoAgfQcaTZXZX4AB7oBo6Un9jWUMF-afUM6mCezc1WyWHp83Yt5iqOCpjntsqo5QYVUD3ioQxE2N.jpg?size=1573x1210&quality=95&type=album "123")
!["123"](https://sun9-west.userapi.com/sun9-8/s/v1/if2/KcbSxNJXSqmvmO-EwLPJEoUiJem9Nm6cIOjS-hoXS3_lGn3iu7BHJBLKQ6iMQtO61BbipG65UADYrj7bthVl7i0Q.jpg?size=2214x1792&quality=95&type=album "123")
!["123"](https://sun9-east.userapi.com/sun9-18/s/v1/if2/sjjxI_Co-F_M5AyHlpdURvoSM9SnIWnIam6Poie4UZsRn8dmEU9kviAKU2JTfFN9OVUIhtAKeFUH7gDRnbxxSr8t.jpg?size=2202x1800&quality=95&type=album "123")
!["123"](https://sun9-east.userapi.com/sun9-44/s/v1/if2/-4HXxr9HlcvzMlzZBe-b1NQ63r3qU21uIZUxKDiZ93VPOa8ZESNcN3lMDSnlmFZZWedU25GjUSREfxoP3ZleG1nH.jpg?size=1802x1792&quality=95&type=album "123")

# 3. Matrix Properties <a name="matrix_props"></a>

## 3.1. The Frobenius Norm <a name="frobenius"></a>



## 3.2. Matrix Multiplication <a name="matrix_mult"></a>



## 3.3. Symmetric and Identity Matrices <a name="sym_identity_matrix"></a>



## 3.4. Matrix Multiplication Exercises <a name="matrix_mult_ex"></a>



## 3.5. Matrix Inversion <a name="matrix_invesrion"></a>



## 3.6. Diagonal Matrices <a name="diagonal_m"></a>



## 3.7. Orthogonal Matrices <a name="orthogonal_matrix"></a>



## 3.8. Orthogonal Matrix Exercises <a name="orthogonal_matrix_ex"></a>

