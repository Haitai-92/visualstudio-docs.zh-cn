---
title: 托管代码的“扩展的设计准则规则”规则集
ms.date: 11/04/2016
ms.prod: visual-studio-dev15
ms.technology: vs-ide-code-analysis
ms.topic: reference
ms.assetid: a338caf2-b75d-4f23-a0f9-3024fa0bceac
author: gewarren
ms.author: gewarren
manager: douge
ms.workload:
- dotnet
ms.openlocfilehash: 2842db460d0a8e3a31921d80cf4a0c3ea0bbc847
ms.sourcegitcommit: e13e61ddea6032a8282abe16131d9e136a927984
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2018
ms.locfileid: "31927095"
---
# <a name="extended-design-guidelines-rules-rule-set-for-managed-code"></a>托管代码的“扩展的设计准则规则”规则集
Microsoft 扩展的设计准则规则规则集扩展基本设计准则规则，以最大化报告的可用性和可维护性问题。 额外的强调置于命名规则。 你应考虑包含此设置，如果你的项目包括库代码，或者如果你想要强制实施有关编写代码容易维护的最高标准的规则。

 扩展的设计准则规则包括所有的 Microsoft 基本设计准则规则。 基本设计准则规则包括所有 Microsoft 最少量建议规则。 有关详细信息，请参阅[的托管代码的基本设计准则规则规则设置](../code-quality/basic-design-guideline-rules-rule-set-for-managed-code.md)和[托管建议规则规则设置对于托管代码](../code-quality/managed-recommended-rules-rule-set-for-managed-code.md)

 下表介绍在 Microsoft 扩展的设计准则规则规则集中的所有规则。

|规则|描述|
|----------|-----------------|
|[CA1001](../code-quality/ca1001-types-that-own-disposable-fields-should-be-disposable.md)|具有可释放字段的类型应该是可释放的|
|[CA1009](../code-quality/ca1009-declare-event-handlers-correctly.md)|正确声明事件处理程序|
|[CA1016](../code-quality/ca1016-mark-assemblies-with-assemblyversionattribute.md)|用 AssemblyVersionAttribute 标记程序集|
|[CA1033](../code-quality/ca1033-interface-methods-should-be-callable-by-child-types.md)|接口方法应可由子类型调用|
|[CA1049](../code-quality/ca1049-types-that-own-native-resources-should-be-disposable.md)|拥有本机资源的类型应是可释放的|
|[CA1060](../code-quality/ca1060-move-p-invokes-to-nativemethods-class.md)|将 P/Invoke 移动到 NativeMethods 类|
|[CA1061](../code-quality/ca1061-do-not-hide-base-class-methods.md)|不要隐藏基类方法|
|[CA1063](../code-quality/ca1063-implement-idisposable-correctly.md)|正确实现 IDisposable|
|[CA1065](../code-quality/ca1065-do-not-raise-exceptions-in-unexpected-locations.md)|不要在意外的位置引发异常|
|[CA1301](../code-quality/ca1301-avoid-duplicate-accelerators.md)|避免快捷键重复|
|[CA1400](../code-quality/ca1400-p-invoke-entry-points-should-exist.md)|P/Invoke 入口点应该存在|
|[CA1401](../code-quality/ca1401-p-invokes-should-not-be-visible.md)|P/Invokes 应该是不可见的|
|[CA1403](../code-quality/ca1403-auto-layout-types-should-not-be-com-visible.md)|自动布局类型不应对 COM 可见|
|[CA1404](../code-quality/ca1404-call-getlasterror-immediately-after-p-invoke.md)|紧接在 P/Invoke 之后调用 GetLastError|
|[CA1405](../code-quality/ca1405-com-visible-type-base-types-should-be-com-visible.md)|COM 可见类型的基类型应对 COM 可见|
|[CA1410](../code-quality/ca1410-com-registration-methods-should-be-matched.md)|应对 COM 注册方法进行匹配|
|[CA1415](../code-quality/ca1415-declare-p-invokes-correctly.md)|正确声明 P/Invoke|
|[CA1821](../code-quality/ca1821-remove-empty-finalizers.md)|移除空终结器|
|[CA1900](../code-quality/ca1900-value-type-fields-should-be-portable.md)|值类型字段应为可移植字段|
|[CA1901](../code-quality/ca1901-p-invoke-declarations-should-be-portable.md)|P/Invoke 声明应为可移植声明|
|[CA2002](../code-quality/ca2002-do-not-lock-on-objects-with-weak-identity.md)|不要锁定具有弱标识的对象|
|[CA2100](../code-quality/ca2100-review-sql-queries-for-security-vulnerabilities.md)|检查 SQL 查询是否存在安全漏洞|
|[CA2101](../code-quality/ca2101-specify-marshaling-for-p-invoke-string-arguments.md)|指定对 P/Invoke 字符串自变量进行封送处理|
|[CA2108](../code-quality/ca2108-review-declarative-security-on-value-types.md)|检查有关值类型的声明性安全|
|[CA2111](../code-quality/ca2111-pointers-should-not-be-visible.md)|指针应为不可见|
|[CA2112](../code-quality/ca2112-secured-types-should-not-expose-fields.md)|受保护的类型不应公开字段|
|[CA2114](../code-quality/ca2114-method-security-should-be-a-superset-of-type.md)|方法安全性应是类型安全性的超集|
|[CA2116](../code-quality/ca2116-aptca-methods-should-only-call-aptca-methods.md)|APTCA 方法应只调用 APTCA 方法|
|[CA2117](../code-quality/ca2117-aptca-types-should-only-extend-aptca-base-types.md)|APTCA 类型应只扩展 APTCA 基类型|
|[CA2122](../code-quality/ca2122-do-not-indirectly-expose-methods-with-link-demands.md)|不要使用链接请求间接公开方法|
|[CA2123](../code-quality/ca2123-override-link-demands-should-be-identical-to-base.md)|重写链接请求应与基相同|
|[CA2124](../code-quality/ca2124-wrap-vulnerable-finally-clauses-in-outer-try.md)|在外部 try 块中包装易受攻击的 finally 子句|
|[CA2126](../code-quality/ca2126-type-link-demands-require-inheritance-demands.md)|类型链接请求需要继承请求|
|[CA2131](../code-quality/ca2131-security-critical-types-may-not-participate-in-type-equivalence.md)|安全关键类型不能参与类型等效|
|[CA2132](../code-quality/ca2132-default-constructors-must-be-at-least-as-critical-as-base-type-default-constructors.md)|默认构造函数必须至少与基类型默认构造函数为关键|
|[CA2133](../code-quality/ca2133-delegates-must-bind-to-methods-with-consistent-transparency.md)|委托必须绑定到具有一致透明度的方法|
|[CA2134](../code-quality/ca2134-methods-must-keep-consistent-transparency-when-overriding-base-methods.md)|在重写基方法时，方法必须保持一致的透明度|
|[CA2137](../code-quality/ca2137-transparent-methods-must-contain-only-verifiable-il.md)|透明方法只能包含可验证的 IL|
|[CA2138](../code-quality/ca2138-transparent-methods-must-not-call-methods-with-the-suppressunmanagedcodesecurity-attribute.md)|透明方法不得调用具有 SuppressUnmanagedCodeSecurity 特性的方法|
|[CA2140](../code-quality/ca2140-transparent-code-must-not-reference-security-critical-items.md)|透明代码不得引用安全关键项|
|[CA2141](../code-quality/ca2141-transparent-methods-must-not-satisfy-linkdemands.md)|透明方法不得满足 LinkDemand|
|[CA2146](../code-quality/ca2146-types-must-be-at-least-as-critical-as-their-base-types-and-interfaces.md)|类型必须是至少与其基类型和接口一样关键|
|[CA2147](../code-quality/ca2147-transparent-methods-may-not-use-security-asserts.md)|透明方法不得使用安全断言|
|[CA2149](../code-quality/ca2149-transparent-methods-must-not-call-into-native-code.md)|透明方法不得调入本机代码|
|[CA2200](../code-quality/ca2200-rethrow-to-preserve-stack-details.md)|再次引发以保留堆栈详细信息|
|[CA2202](../code-quality/ca2202-do-not-dispose-objects-multiple-times.md)|不要多次释放对象|
|[CA2207](../code-quality/ca2207-initialize-value-type-static-fields-inline.md)|以内联方式初始化值类型的静态字段|
|[CA2212](../code-quality/ca2212-do-not-mark-serviced-components-with-webmethod.md)|不要使用 WebMethod 标记服务组件|
|[CA2213](../code-quality/ca2213-disposable-fields-should-be-disposed.md)|应释放可释放的字段|
|[CA2214](../code-quality/ca2214-do-not-call-overridable-methods-in-constructors.md)|不要在构造函数中调用可重写的方法|
|[CA2216](../code-quality/ca2216-disposable-types-should-declare-finalizer.md)|可释放类型应声明终结器|
|[CA2220](../code-quality/ca2220-finalizers-should-call-base-class-finalizer.md)|终结器应调用基类的终结器|
|[CA2229](../code-quality/ca2229-implement-serialization-constructors.md)|实现序列化构造函数|
|[CA2231](../code-quality/ca2231-overload-operator-equals-on-overriding-valuetype-equals.md)|重写 ValueType.Equals 时应重载相等运算符|
|[CA2232](../code-quality/ca2232-mark-windows-forms-entry-points-with-stathread.md)|使用 STAThread 标记 Windows 窗体的入口点|
|[CA2235](../code-quality/ca2235-mark-all-non-serializable-fields.md)|标记所有不可序列化的字段|
|[CA2236](../code-quality/ca2236-call-base-class-methods-on-iserializable-types.md)|对 ISerializable 类型调用基类方法|
|[CA2237](../code-quality/ca2237-mark-iserializable-types-with-serializableattribute.md)|用 SerializableAttribute 标记 ISerializable 类型|
|[CA2238](../code-quality/ca2238-implement-serialization-methods-correctly.md)|正确实现序列化方法|
|[CA2240](../code-quality/ca2240-implement-iserializable-correctly.md)|正确实现 ISerializable|
|[CA2241](../code-quality/ca2241-provide-correct-arguments-to-formatting-methods.md)|为格式化方法提供正确的自变量|
|[CA2242](../code-quality/ca2242-test-for-nan-correctly.md)|正确测试 NaN|
|[CA1000](../code-quality/ca1000-do-not-declare-static-members-on-generic-types.md)|不要在泛型类型中声明静态成员|
|[CA1002](../code-quality/ca1002-do-not-expose-generic-lists.md)|不要公开泛型列表|
|[CA1003](../code-quality/ca1003-use-generic-event-handler-instances.md)|使用泛型事件处理程序实例|
|[CA1004](../code-quality/ca1004-generic-methods-should-provide-type-parameter.md)|泛型方法应提供类型参数|
|[CA1005](../code-quality/ca1005-avoid-excessive-parameters-on-generic-types.md)|避免泛型类型参数过多|
|[CA1006](../code-quality/ca1006-do-not-nest-generic-types-in-member-signatures.md)|不要嵌套成员签名中的泛型类型|
|[CA1007](../code-quality/ca1007-use-generics-where-appropriate.md)|在适用处使用泛型|
|[CA1008](../code-quality/ca1008-enums-should-have-zero-value.md)|枚举应具有零值|
|[CA1010](../code-quality/ca1010-collections-should-implement-generic-interface.md)|集合应实现泛型接口|
|[CA1011](../code-quality/ca1011-consider-passing-base-types-as-parameters.md)|请考虑将基类型作为参数传递|
|[CA1012](../code-quality/ca1012-abstract-types-should-not-have-constructors.md)|抽象类型不应具有构造函数|
|[CA1013](../code-quality/ca1013-overload-operator-equals-on-overloading-add-and-subtract.md)|重载重载相等运算符重载加法方法和减法|
|[CA1014](../code-quality/ca1014-mark-assemblies-with-clscompliantattribute.md)|用 CLSCompliantAttribute 标记程序集|
|[CA1017](../code-quality/ca1017-mark-assemblies-with-comvisibleattribute.md)|用 ComVisibleAttribute 标记程序集|
|[CA1018](../code-quality/ca1018-mark-attributes-with-attributeusageattribute.md)|用 AttributeUsageAttribute 标记特性|
|[CA1019](../code-quality/ca1019-define-accessors-for-attribute-arguments.md)|定义特性自变量的访问器|
|[CA1023](../code-quality/ca1023-indexers-should-not-be-multidimensional.md)|索引器不应是多维|
|[CA1024](../code-quality/ca1024-use-properties-where-appropriate.md)|在适用处使用属性|
|[CA1025](../code-quality/ca1025-replace-repetitive-arguments-with-params-array.md)|使用参数数组替换重复的实参|
|[CA1026](../code-quality/ca1026-default-parameters-should-not-be-used.md)|不应使用默认参数|
|[CA1027](../code-quality/ca1027-mark-enums-with-flagsattribute.md)|用 FlagsAttribute 标记枚举|
|[CA1028](../code-quality/ca1028-enum-storage-should-be-int32.md)|枚举存储应为 Int32|
|[CA1030 在适用处](../code-quality/ca1030-use-events-where-appropriate.md)|在适用处使用事件|
|[CA1031](../code-quality/ca1031-do-not-catch-general-exception-types.md)|不要捕捉一般异常类型|
|[CA1032](../code-quality/ca1032-implement-standard-exception-constructors.md)|实现标准异常构造函数|
|[CA1034](../code-quality/ca1034-nested-types-should-not-be-visible.md)|嵌套的类型不应是可见|
|[CA1035](../code-quality/ca1035-icollection-implementations-have-strongly-typed-members.md)|ICollection 实现含有强类型成员|
|[CA1036](../code-quality/ca1036-override-methods-on-comparable-types.md)|重写可比较类型的方法|
|[CA1038](../code-quality/ca1038-enumerators-should-be-strongly-typed.md)|枚举数应强类型化|
|[CA1039](../code-quality/ca1039-lists-are-strongly-typed.md)|强类型列表|
|[CA1041](../code-quality/ca1041-provide-obsoleteattribute-message.md)|提供 ObsoleteAttribute 消息|
|[CA1043](../code-quality/ca1043-use-integral-or-string-argument-for-indexers.md)|将整型或字符串自变量用于索引器|
|[CA1044](../code-quality/ca1044-properties-should-not-be-write-only.md)|不应只写属性。|
|[CA1046](../code-quality/ca1046-do-not-overload-operator-equals-on-reference-types.md)|不要重载引用类型重载相等运算符|
|[CA1047](../code-quality/ca1047-do-not-declare-protected-members-in-sealed-types.md)|不要声明在密封类型中的受保护的成员|
|[CA1048](../code-quality/ca1048-do-not-declare-virtual-members-in-sealed-types.md)|不要声明在密封类型中的虚拟成员|
|[CA1050](../code-quality/ca1050-declare-types-in-namespaces.md)|在命名空间中声明类型|
|[CA1051](../code-quality/ca1051-do-not-declare-visible-instance-fields.md)|不要声明可见实例字段|
|[CA1052](../code-quality/ca1052-static-holder-types-should-be-sealed.md)|应密封静态容器类型|
|[CA1053](../code-quality/ca1053-static-holder-types-should-not-have-constructors.md)|静态容器类型不应具有构造函数|
|[CA1054](../code-quality/ca1054-uri-parameters-should-not-be-strings.md)|URI 参数不应为字符串|
|[CA1055](../code-quality/ca1055-uri-return-values-should-not-be-strings.md)|URI 返回值不应为字符串|
|[CA1056](../code-quality/ca1056-uri-properties-should-not-be-strings.md)|URI 属性不应为字符串|
|[CA1057](../code-quality/ca1057-string-uri-overloads-call-system-uri-overloads.md)|字符串 URI 重载调用 System.Uri 重载|
|[CA1058](../code-quality/ca1058-types-should-not-extend-certain-base-types.md)|类型不应扩展某些基类型|
|[CA1059](../code-quality/ca1059-members-should-not-expose-certain-concrete-types.md)|成员不应公开某些具体类型|
|[CA1064](../code-quality/ca1064-exceptions-should-be-public.md)|异常应该是公共的|
|[CA1500](../code-quality/ca1500-variable-names-should-not-match-field-names.md)|变量名不应与字段名称|
|[CA1502](../code-quality/ca1502-avoid-excessive-complexity.md)|避免过度复杂|
|[CA1708](../code-quality/ca1708-identifiers-should-differ-by-more-than-case.md)|标识符不应不同大小写进行区分|
|[CA1716](../code-quality/ca1716-identifiers-should-not-match-keywords.md)|标识符不应与关键字|
|[CA1801](../code-quality/ca1801-review-unused-parameters.md)|查看未使用的参数|
|[CA1804](../code-quality/ca1804-remove-unused-locals.md)|删除未使用的局部变量|
|[CA1809](../code-quality/ca1809-avoid-excessive-locals.md)|避免过多的局部变量|
|[CA1810](../code-quality/ca1810-initialize-reference-type-static-fields-inline.md)|引用类型的静态字段以内联方式初始化|
|[CA1811](../code-quality/ca1811-avoid-uncalled-private-code.md)|避免使用未调用的私有代码|
|[CA1812](../code-quality/ca1812-avoid-uninstantiated-internal-classes.md)|避免未实例化的内部类|
|[CA1813](../code-quality/ca1813-avoid-unsealed-attributes.md)|避免未密封的特性|
|[CA1814](../code-quality/ca1814-prefer-jagged-arrays-over-multidimensional.md)|更愿意交错的数组，而多维|
|[CA1815](../code-quality/ca1815-override-equals-and-operator-equals-on-value-types.md)|重写 equals 和相等运算符的值类型|
|[CA1819](../code-quality/ca1819-properties-should-not-return-arrays.md)|属性不应返回数组|
|[CA1820](../code-quality/ca1820-test-for-empty-strings-using-string-length.md)|测试有空字符串使用字符串长度|
|[CA1822](../code-quality/ca1822-mark-members-as-static.md)|将成员标记为 static|
|[CA1823](../code-quality/ca1823-avoid-unused-private-fields.md)|避免未使用的私有字段|
|[CA2201](../code-quality/ca2201-do-not-raise-reserved-exception-types.md)|不会引发保留的异常类型|
|[CA2205](../code-quality/ca2205-use-managed-equivalents-of-win32-api.md)|使用 Win32 API 的托管等效项|
|[CA2208](../code-quality/ca2208-instantiate-argument-exceptions-correctly.md)|正确实例化自变量异常|
|[CA2211](../code-quality/ca2211-non-constant-fields-should-not-be-visible.md)|非常量字段不应是可见|
|[CA2217](../code-quality/ca2217-do-not-mark-enums-with-flagsattribute.md)|不用 FlagsAttribute 标记枚举|
|[CA2219](../code-quality/ca2219-do-not-raise-exceptions-in-exception-clauses.md)|不会引发异常子句中的异常|
|[CA2221](../code-quality/ca2221-finalizers-should-be-protected.md)|终结器应受到保护|
|[CA2222](../code-quality/ca2222-do-not-decrease-inherited-member-visibility.md)|不要递减继承的成员的可见性|
|[CA2223](../code-quality/ca2223-members-should-differ-by-more-than-return-type.md)|成员不应通过多个返回类型不同|
|[CA2224](../code-quality/ca2224-override-equals-on-overloading-operator-equals.md)|重写 equals 方法重载相等运算符|
|[CA2225](../code-quality/ca2225-operator-overloads-have-named-alternates.md)|运算符重载具有命名的备用项|
|[CA2226](../code-quality/ca2226-operators-should-have-symmetrical-overloads.md)|运算符应有对称重载|
|[CA2227](../code-quality/ca2227-collection-properties-should-be-read-only.md)|集合属性应为只读|
|[CA2230](../code-quality/ca2230-use-params-for-variable-arguments.md)|对变量自变量使用 params|
|[CA2234](../code-quality/ca2234-pass-system-uri-objects-instead-of-strings.md)|传递 System.Uri 对象，而不是字符串|
|[CA2239](../code-quality/ca2239-provide-deserialization-methods-for-optional-fields.md)|提供为可选字段的反序列化方法|
|[CA1020](../code-quality/ca1020-avoid-namespaces-with-few-types.md)|避免与几种类型的命名空间|
|[CA1021](../code-quality/ca1021-avoid-out-parameters.md)|避免使用 out 参数|
|[CA1040](../code-quality/ca1040-avoid-empty-interfaces.md)|避免使用空接口|
|[CA1045](../code-quality/ca1045-do-not-pass-types-by-reference.md)|不要通过引用传递类型|
|[CA1062](../code-quality/ca1062-validate-arguments-of-public-methods.md)|验证公共方法的参数|
|[CA1501](../code-quality/ca1501-avoid-excessive-inheritance.md)|避免过度继承|
|[CA1504](../code-quality/ca1504-review-misleading-field-names.md)|检查令人误解的字段名|
|[CA1505](../code-quality/ca1505-avoid-unmaintainable-code.md)|避免编写无法维护的代码|
|[CA1506](../code-quality/ca1506-avoid-excessive-class-coupling.md)|避免过度类耦合|
|[CA1700](../code-quality/ca1700-do-not-name-enum-values-reserved.md)|未命名枚举值 Reserved|
|[CA1701](../code-quality/ca1701-resource-string-compound-words-should-be-cased-correctly.md)|资源字符串复合词应采用正确的大小写|
|[CA1702](../code-quality/ca1702-compound-words-should-be-cased-correctly.md)|复合词应采用正确的大小写|
|[CA1703](../code-quality/ca1703-resource-strings-should-be-spelled-correctly.md)|资源字符串应正确拼写|
|[CA1704](../code-quality/ca1704-identifiers-should-be-spelled-correctly.md)|标识符应正确拼写|
|[CA1707](../code-quality/ca1707-identifiers-should-not-contain-underscores.md)|标识符不应包含下划线|
|[CA1709](../code-quality/ca1709-identifiers-should-be-cased-correctly.md)|标识符应采用正确的大小写|
|[CA1710](../code-quality/ca1710-identifiers-should-have-correct-suffix.md)|标识符应具有正确的后缀|
|[CA1711](../code-quality/ca1711-identifiers-should-not-have-incorrect-suffix.md)|标识符不应具有正确的后缀|
|[CA1712](../code-quality/ca1712-do-not-prefix-enum-values-with-type-name.md)|不要使用类型名称的枚举值的前缀|
|[CA1713](../code-quality/ca1713-events-should-not-have-before-or-after-prefix.md)|事件不应具有 before 或 after 前缀|
|[CA1714](../code-quality/ca1714-flags-enums-should-have-plural-names.md)|Flags 枚举应采用复数形式的名称|
|[CA1715](../code-quality/ca1715-identifiers-should-have-correct-prefix.md)|标识符应具有正确的前缀|
|[CA1717](../code-quality/ca1717-only-flagsattribute-enums-should-have-plural-names.md)|只有 FlagsAttribute 枚举应采用复数形式的名称|
|[CA1719](../code-quality/ca1719-parameter-names-should-not-match-member-names.md)|参数名称不应与成员名|
|[CA1720](../code-quality/ca1720-identifiers-should-not-contain-type-names.md)|标识符不应包含类型名称|
|[CA1721](../code-quality/ca1721-property-names-should-not-match-get-methods.md)|属性名不应与 get 方法|
|[CA1722](../code-quality/ca1722-identifiers-should-not-have-incorrect-prefix.md)|标识符不应具有正确的前缀|
|[CA1724](../code-quality/ca1724-type-names-should-not-match-namespaces.md)|类型名称不应与命名空间|
|[CA1725](../code-quality/ca1725-parameter-names-should-match-base-declaration.md)|参数名应与基声明|
|[CA1726](../code-quality/ca1726-use-preferred-terms.md)|使用首选的词条|
|[CA2204](../code-quality/ca2204-literals-should-be-spelled-correctly.md)|应正确拼写文本|