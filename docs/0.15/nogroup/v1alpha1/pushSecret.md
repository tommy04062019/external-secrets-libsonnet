---
permalink: /0.15/nogroup/v1alpha1/pushSecret/
---

# nogroup.v1alpha1.pushSecret



## Index

* [`fn new(name)`](#fn-new)
* [`obj metadata`](#obj-metadata)
  * [`fn withAnnotations(annotations)`](#fn-metadatawithannotations)
  * [`fn withAnnotationsMixin(annotations)`](#fn-metadatawithannotationsmixin)
  * [`fn withClusterName(clusterName)`](#fn-metadatawithclustername)
  * [`fn withCreationTimestamp(creationTimestamp)`](#fn-metadatawithcreationtimestamp)
  * [`fn withDeletionGracePeriodSeconds(deletionGracePeriodSeconds)`](#fn-metadatawithdeletiongraceperiodseconds)
  * [`fn withDeletionTimestamp(deletionTimestamp)`](#fn-metadatawithdeletiontimestamp)
  * [`fn withFinalizers(finalizers)`](#fn-metadatawithfinalizers)
  * [`fn withFinalizersMixin(finalizers)`](#fn-metadatawithfinalizersmixin)
  * [`fn withGenerateName(generateName)`](#fn-metadatawithgeneratename)
  * [`fn withGeneration(generation)`](#fn-metadatawithgeneration)
  * [`fn withLabels(labels)`](#fn-metadatawithlabels)
  * [`fn withLabelsMixin(labels)`](#fn-metadatawithlabelsmixin)
  * [`fn withName(name)`](#fn-metadatawithname)
  * [`fn withNamespace(namespace)`](#fn-metadatawithnamespace)
  * [`fn withOwnerReferences(ownerReferences)`](#fn-metadatawithownerreferences)
  * [`fn withOwnerReferencesMixin(ownerReferences)`](#fn-metadatawithownerreferencesmixin)
  * [`fn withResourceVersion(resourceVersion)`](#fn-metadatawithresourceversion)
  * [`fn withSelfLink(selfLink)`](#fn-metadatawithselflink)
  * [`fn withUid(uid)`](#fn-metadatawithuid)
* [`obj spec`](#obj-spec)
  * [`fn withData(data)`](#fn-specwithdata)
  * [`fn withDataMixin(data)`](#fn-specwithdatamixin)
  * [`fn withDeletionPolicy(deletionPolicy)`](#fn-specwithdeletionpolicy)
  * [`fn withRefreshInterval(refreshInterval)`](#fn-specwithrefreshinterval)
  * [`fn withSecretStoreRefs(secretStoreRefs)`](#fn-specwithsecretstorerefs)
  * [`fn withSecretStoreRefsMixin(secretStoreRefs)`](#fn-specwithsecretstorerefsmixin)
  * [`fn withUpdatePolicy(updatePolicy)`](#fn-specwithupdatepolicy)
  * [`obj spec.data`](#obj-specdata)
    * [`fn withConversionStrategy(conversionStrategy)`](#fn-specdatawithconversionstrategy)
    * [`fn withMetadata(metadata)`](#fn-specdatawithmetadata)
    * [`obj spec.data.match`](#obj-specdatamatch)
      * [`fn withSecretKey(secretKey)`](#fn-specdatamatchwithsecretkey)
      * [`obj spec.data.match.remoteRef`](#obj-specdatamatchremoteref)
        * [`fn withProperty(property)`](#fn-specdatamatchremoterefwithproperty)
        * [`fn withRemoteKey(remoteKey)`](#fn-specdatamatchremoterefwithremotekey)
  * [`obj spec.secretStoreRefs`](#obj-specsecretstorerefs)
    * [`fn withKind(kind)`](#fn-specsecretstorerefswithkind)
    * [`fn withName(name)`](#fn-specsecretstorerefswithname)
    * [`obj spec.secretStoreRefs.labelSelector`](#obj-specsecretstorerefslabelselector)
      * [`fn withMatchExpressions(matchExpressions)`](#fn-specsecretstorerefslabelselectorwithmatchexpressions)
      * [`fn withMatchExpressionsMixin(matchExpressions)`](#fn-specsecretstorerefslabelselectorwithmatchexpressionsmixin)
      * [`fn withMatchLabels(matchLabels)`](#fn-specsecretstorerefslabelselectorwithmatchlabels)
      * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specsecretstorerefslabelselectorwithmatchlabelsmixin)
      * [`obj spec.secretStoreRefs.labelSelector.matchExpressions`](#obj-specsecretstorerefslabelselectormatchexpressions)
        * [`fn withKey(key)`](#fn-specsecretstorerefslabelselectormatchexpressionswithkey)
        * [`fn withOperator(operator)`](#fn-specsecretstorerefslabelselectormatchexpressionswithoperator)
        * [`fn withValues(values)`](#fn-specsecretstorerefslabelselectormatchexpressionswithvalues)
        * [`fn withValuesMixin(values)`](#fn-specsecretstorerefslabelselectormatchexpressionswithvaluesmixin)
  * [`obj spec.selector`](#obj-specselector)
    * [`obj spec.selector.generatorRef`](#obj-specselectorgeneratorref)
      * [`fn withApiVersion(apiVersion)`](#fn-specselectorgeneratorrefwithapiversion)
      * [`fn withKind(kind)`](#fn-specselectorgeneratorrefwithkind)
      * [`fn withName(name)`](#fn-specselectorgeneratorrefwithname)
    * [`obj spec.selector.secret`](#obj-specselectorsecret)
      * [`fn withName(name)`](#fn-specselectorsecretwithname)
      * [`obj spec.selector.secret.selector`](#obj-specselectorsecretselector)
        * [`fn withMatchExpressions(matchExpressions)`](#fn-specselectorsecretselectorwithmatchexpressions)
        * [`fn withMatchExpressionsMixin(matchExpressions)`](#fn-specselectorsecretselectorwithmatchexpressionsmixin)
        * [`fn withMatchLabels(matchLabels)`](#fn-specselectorsecretselectorwithmatchlabels)
        * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specselectorsecretselectorwithmatchlabelsmixin)
        * [`obj spec.selector.secret.selector.matchExpressions`](#obj-specselectorsecretselectormatchexpressions)
          * [`fn withKey(key)`](#fn-specselectorsecretselectormatchexpressionswithkey)
          * [`fn withOperator(operator)`](#fn-specselectorsecretselectormatchexpressionswithoperator)
          * [`fn withValues(values)`](#fn-specselectorsecretselectormatchexpressionswithvalues)
          * [`fn withValuesMixin(values)`](#fn-specselectorsecretselectormatchexpressionswithvaluesmixin)
  * [`obj spec.template`](#obj-spectemplate)
    * [`fn withData(data)`](#fn-spectemplatewithdata)
    * [`fn withDataMixin(data)`](#fn-spectemplatewithdatamixin)
    * [`fn withEngineVersion(engineVersion)`](#fn-spectemplatewithengineversion)
    * [`fn withMergePolicy(mergePolicy)`](#fn-spectemplatewithmergepolicy)
    * [`fn withTemplateFrom(templateFrom)`](#fn-spectemplatewithtemplatefrom)
    * [`fn withTemplateFromMixin(templateFrom)`](#fn-spectemplatewithtemplatefrommixin)
    * [`fn withType(type)`](#fn-spectemplatewithtype)
    * [`obj spec.template.metadata`](#obj-spectemplatemetadata)
      * [`fn withAnnotations(annotations)`](#fn-spectemplatemetadatawithannotations)
      * [`fn withAnnotationsMixin(annotations)`](#fn-spectemplatemetadatawithannotationsmixin)
      * [`fn withLabels(labels)`](#fn-spectemplatemetadatawithlabels)
      * [`fn withLabelsMixin(labels)`](#fn-spectemplatemetadatawithlabelsmixin)
    * [`obj spec.template.templateFrom`](#obj-spectemplatetemplatefrom)
      * [`fn withLiteral(literal)`](#fn-spectemplatetemplatefromwithliteral)
      * [`fn withTarget(target)`](#fn-spectemplatetemplatefromwithtarget)
      * [`obj spec.template.templateFrom.configMap`](#obj-spectemplatetemplatefromconfigmap)
        * [`fn withItems(items)`](#fn-spectemplatetemplatefromconfigmapwithitems)
        * [`fn withItemsMixin(items)`](#fn-spectemplatetemplatefromconfigmapwithitemsmixin)
        * [`fn withName(name)`](#fn-spectemplatetemplatefromconfigmapwithname)
        * [`obj spec.template.templateFrom.configMap.items`](#obj-spectemplatetemplatefromconfigmapitems)
          * [`fn withKey(key)`](#fn-spectemplatetemplatefromconfigmapitemswithkey)
          * [`fn withTemplateAs(templateAs)`](#fn-spectemplatetemplatefromconfigmapitemswithtemplateas)
      * [`obj spec.template.templateFrom.secret`](#obj-spectemplatetemplatefromsecret)
        * [`fn withItems(items)`](#fn-spectemplatetemplatefromsecretwithitems)
        * [`fn withItemsMixin(items)`](#fn-spectemplatetemplatefromsecretwithitemsmixin)
        * [`fn withName(name)`](#fn-spectemplatetemplatefromsecretwithname)
        * [`obj spec.template.templateFrom.secret.items`](#obj-spectemplatetemplatefromsecretitems)
          * [`fn withKey(key)`](#fn-spectemplatetemplatefromsecretitemswithkey)
          * [`fn withTemplateAs(templateAs)`](#fn-spectemplatetemplatefromsecretitemswithtemplateas)

## Fields

### fn new

```ts
new(name)
```

new returns an instance of PushSecret

## obj metadata

"ObjectMeta is metadata that all persisted resources must have, which includes all objects users must create."

### fn metadata.withAnnotations

```ts
withAnnotations(annotations)
```

"Annotations is an unstructured key value map stored with a resource that may be set by external tools to store and retrieve arbitrary metadata. They are not queryable and should be preserved when modifying objects. More info: http://kubernetes.io/docs/user-guide/annotations"

### fn metadata.withAnnotationsMixin

```ts
withAnnotationsMixin(annotations)
```

"Annotations is an unstructured key value map stored with a resource that may be set by external tools to store and retrieve arbitrary metadata. They are not queryable and should be preserved when modifying objects. More info: http://kubernetes.io/docs/user-guide/annotations"

**Note:** This function appends passed data to existing values

### fn metadata.withClusterName

```ts
withClusterName(clusterName)
```

"The name of the cluster which the object belongs to. This is used to distinguish resources with same name and namespace in different clusters. This field is not set anywhere right now and apiserver is going to ignore it if set in create or update request."

### fn metadata.withCreationTimestamp

```ts
withCreationTimestamp(creationTimestamp)
```

"Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers."

### fn metadata.withDeletionGracePeriodSeconds

```ts
withDeletionGracePeriodSeconds(deletionGracePeriodSeconds)
```

"Number of seconds allowed for this object to gracefully terminate before it will be removed from the system. Only set when deletionTimestamp is also set. May only be shortened. Read-only."

### fn metadata.withDeletionTimestamp

```ts
withDeletionTimestamp(deletionTimestamp)
```

"Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers."

### fn metadata.withFinalizers

```ts
withFinalizers(finalizers)
```

"Must be empty before the object is deleted from the registry. Each entry is an identifier for the responsible component that will remove the entry from the list. If the deletionTimestamp of the object is non-nil, entries in this list can only be removed. Finalizers may be processed and removed in any order.  Order is NOT enforced because it introduces significant risk of stuck finalizers. finalizers is a shared field, any actor with permission can reorder it. If the finalizer list is processed in order, then this can lead to a situation in which the component responsible for the first finalizer in the list is waiting for a signal (field value, external system, or other) produced by a component responsible for a finalizer later in the list, resulting in a deadlock. Without enforced ordering finalizers are free to order amongst themselves and are not vulnerable to ordering changes in the list."

### fn metadata.withFinalizersMixin

```ts
withFinalizersMixin(finalizers)
```

"Must be empty before the object is deleted from the registry. Each entry is an identifier for the responsible component that will remove the entry from the list. If the deletionTimestamp of the object is non-nil, entries in this list can only be removed. Finalizers may be processed and removed in any order.  Order is NOT enforced because it introduces significant risk of stuck finalizers. finalizers is a shared field, any actor with permission can reorder it. If the finalizer list is processed in order, then this can lead to a situation in which the component responsible for the first finalizer in the list is waiting for a signal (field value, external system, or other) produced by a component responsible for a finalizer later in the list, resulting in a deadlock. Without enforced ordering finalizers are free to order amongst themselves and are not vulnerable to ordering changes in the list."

**Note:** This function appends passed data to existing values

### fn metadata.withGenerateName

```ts
withGenerateName(generateName)
```

"GenerateName is an optional prefix, used by the server, to generate a unique name ONLY IF the Name field has not been provided. If this field is used, the name returned to the client will be different than the name passed. This value will also be combined with a unique suffix. The provided value has the same validation rules as the Name field, and may be truncated by the length of the suffix required to make the value unique on the server.\n\nIf this field is specified and the generated name exists, the server will NOT return a 409 - instead, it will either return 201 Created or 500 with Reason ServerTimeout indicating a unique name could not be found in the time allotted, and the client should retry (optionally after the time indicated in the Retry-After header).\n\nApplied only if Name is not specified. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#idempotency"

### fn metadata.withGeneration

```ts
withGeneration(generation)
```

"A sequence number representing a specific generation of the desired state. Populated by the system. Read-only."

### fn metadata.withLabels

```ts
withLabels(labels)
```

"Map of string keys and values that can be used to organize and categorize (scope and select) objects. May match selectors of replication controllers and services. More info: http://kubernetes.io/docs/user-guide/labels"

### fn metadata.withLabelsMixin

```ts
withLabelsMixin(labels)
```

"Map of string keys and values that can be used to organize and categorize (scope and select) objects. May match selectors of replication controllers and services. More info: http://kubernetes.io/docs/user-guide/labels"

**Note:** This function appends passed data to existing values

### fn metadata.withName

```ts
withName(name)
```

"Name must be unique within a namespace. Is required when creating resources, although some resources may allow a client to request the generation of an appropriate name automatically. Name is primarily intended for creation idempotence and configuration definition. Cannot be updated. More info: http://kubernetes.io/docs/user-guide/identifiers#names"

### fn metadata.withNamespace

```ts
withNamespace(namespace)
```

"Namespace defines the space within which each name must be unique. An empty namespace is equivalent to the \"default\" namespace, but \"default\" is the canonical representation. Not all objects are required to be scoped to a namespace - the value of this field for those objects will be empty.\n\nMust be a DNS_LABEL. Cannot be updated. More info: http://kubernetes.io/docs/user-guide/namespaces"

### fn metadata.withOwnerReferences

```ts
withOwnerReferences(ownerReferences)
```

"List of objects depended by this object. If ALL objects in the list have been deleted, this object will be garbage collected. If this object is managed by a controller, then an entry in this list will point to this controller, with the controller field set to true. There cannot be more than one managing controller."

### fn metadata.withOwnerReferencesMixin

```ts
withOwnerReferencesMixin(ownerReferences)
```

"List of objects depended by this object. If ALL objects in the list have been deleted, this object will be garbage collected. If this object is managed by a controller, then an entry in this list will point to this controller, with the controller field set to true. There cannot be more than one managing controller."

**Note:** This function appends passed data to existing values

### fn metadata.withResourceVersion

```ts
withResourceVersion(resourceVersion)
```

"An opaque value that represents the internal version of this object that can be used by clients to determine when objects have changed. May be used for optimistic concurrency, change detection, and the watch operation on a resource or set of resources. Clients must treat these values as opaque and passed unmodified back to the server. They may only be valid for a particular resource or set of resources.\n\nPopulated by the system. Read-only. Value must be treated as opaque by clients and . More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#concurrency-control-and-consistency"

### fn metadata.withSelfLink

```ts
withSelfLink(selfLink)
```

"SelfLink is a URL representing this object. Populated by the system. Read-only.\n\nDEPRECATED Kubernetes will stop propagating this field in 1.20 release and the field is planned to be removed in 1.21 release."

### fn metadata.withUid

```ts
withUid(uid)
```

"UID is the unique in time and space value for this object. It is typically generated by the server on successful creation of a resource and is not allowed to change on PUT operations.\n\nPopulated by the system. Read-only. More info: http://kubernetes.io/docs/user-guide/identifiers#uids"

## obj spec

"PushSecretSpec configures the behavior of the PushSecret."

### fn spec.withData

```ts
withData(data)
```

"Secret Data that should be pushed to providers"

### fn spec.withDataMixin

```ts
withDataMixin(data)
```

"Secret Data that should be pushed to providers"

**Note:** This function appends passed data to existing values

### fn spec.withDeletionPolicy

```ts
withDeletionPolicy(deletionPolicy)
```

"Deletion Policy to handle Secrets in the provider."

### fn spec.withRefreshInterval

```ts
withRefreshInterval(refreshInterval)
```

"The Interval to which External Secrets will try to push a secret definition"

### fn spec.withSecretStoreRefs

```ts
withSecretStoreRefs(secretStoreRefs)
```



### fn spec.withSecretStoreRefsMixin

```ts
withSecretStoreRefsMixin(secretStoreRefs)
```



**Note:** This function appends passed data to existing values

### fn spec.withUpdatePolicy

```ts
withUpdatePolicy(updatePolicy)
```

"UpdatePolicy to handle Secrets in the provider."

## obj spec.data

"Secret Data that should be pushed to providers"

### fn spec.data.withConversionStrategy

```ts
withConversionStrategy(conversionStrategy)
```

"Used to define a conversion Strategy for the secret keys"

### fn spec.data.withMetadata

```ts
withMetadata(metadata)
```

"Metadata is metadata attached to the secret.\nThe structure of metadata is provider specific, please look it up in the provider documentation."

## obj spec.data.match

"Match a given Secret Key to be pushed to the provider."

### fn spec.data.match.withSecretKey

```ts
withSecretKey(secretKey)
```

"Secret Key to be pushed"

## obj spec.data.match.remoteRef

"Remote Refs to push to providers."

### fn spec.data.match.remoteRef.withProperty

```ts
withProperty(property)
```

"Name of the property in the resulting secret"

### fn spec.data.match.remoteRef.withRemoteKey

```ts
withRemoteKey(remoteKey)
```

"Name of the resulting provider secret."

## obj spec.secretStoreRefs



### fn spec.secretStoreRefs.withKind

```ts
withKind(kind)
```

"Kind of the SecretStore resource (SecretStore or ClusterSecretStore)"

### fn spec.secretStoreRefs.withName

```ts
withName(name)
```

"Optionally, sync to the SecretStore of the given name"

## obj spec.secretStoreRefs.labelSelector

"Optionally, sync to secret stores with label selector"

### fn spec.secretStoreRefs.labelSelector.withMatchExpressions

```ts
withMatchExpressions(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.secretStoreRefs.labelSelector.withMatchExpressionsMixin

```ts
withMatchExpressionsMixin(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

**Note:** This function appends passed data to existing values

### fn spec.secretStoreRefs.labelSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels\nmap is equivalent to an element of matchExpressions, whose key field is \"key\", the\noperator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

### fn spec.secretStoreRefs.labelSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels\nmap is equivalent to an element of matchExpressions, whose key field is \"key\", the\noperator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

**Note:** This function appends passed data to existing values

## obj spec.secretStoreRefs.labelSelector.matchExpressions

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.secretStoreRefs.labelSelector.matchExpressions.withKey

```ts
withKey(key)
```

"key is the label key that the selector applies to."

### fn spec.secretStoreRefs.labelSelector.matchExpressions.withOperator

```ts
withOperator(operator)
```

"operator represents a key's relationship to a set of values.\nValid operators are In, NotIn, Exists and DoesNotExist."

### fn spec.secretStoreRefs.labelSelector.matchExpressions.withValues

```ts
withValues(values)
```

"values is an array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. This array is replaced during a strategic\nmerge patch."

### fn spec.secretStoreRefs.labelSelector.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"values is an array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. This array is replaced during a strategic\nmerge patch."

**Note:** This function appends passed data to existing values

## obj spec.selector

"The Secret Selector (k8s source) for the Push Secret"

## obj spec.selector.generatorRef

"Point to a generator to create a Secret."

### fn spec.selector.generatorRef.withApiVersion

```ts
withApiVersion(apiVersion)
```

"Specify the apiVersion of the generator resource"

### fn spec.selector.generatorRef.withKind

```ts
withKind(kind)
```

"Specify the Kind of the generator resource"

### fn spec.selector.generatorRef.withName

```ts
withName(name)
```

"Specify the name of the generator resource"

## obj spec.selector.secret

"Select a Secret to Push."

### fn spec.selector.secret.withName

```ts
withName(name)
```

"Name of the Secret.\nThe Secret must exist in the same namespace as the PushSecret manifest."

## obj spec.selector.secret.selector

"Selector chooses secrets using a labelSelector."

### fn spec.selector.secret.selector.withMatchExpressions

```ts
withMatchExpressions(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.selector.secret.selector.withMatchExpressionsMixin

```ts
withMatchExpressionsMixin(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

**Note:** This function appends passed data to existing values

### fn spec.selector.secret.selector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels\nmap is equivalent to an element of matchExpressions, whose key field is \"key\", the\noperator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

### fn spec.selector.secret.selector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels\nmap is equivalent to an element of matchExpressions, whose key field is \"key\", the\noperator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

**Note:** This function appends passed data to existing values

## obj spec.selector.secret.selector.matchExpressions

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.selector.secret.selector.matchExpressions.withKey

```ts
withKey(key)
```

"key is the label key that the selector applies to."

### fn spec.selector.secret.selector.matchExpressions.withOperator

```ts
withOperator(operator)
```

"operator represents a key's relationship to a set of values.\nValid operators are In, NotIn, Exists and DoesNotExist."

### fn spec.selector.secret.selector.matchExpressions.withValues

```ts
withValues(values)
```

"values is an array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. This array is replaced during a strategic\nmerge patch."

### fn spec.selector.secret.selector.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"values is an array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. This array is replaced during a strategic\nmerge patch."

**Note:** This function appends passed data to existing values

## obj spec.template

"Template defines a blueprint for the created Secret resource."

### fn spec.template.withData

```ts
withData(data)
```



### fn spec.template.withDataMixin

```ts
withDataMixin(data)
```



**Note:** This function appends passed data to existing values

### fn spec.template.withEngineVersion

```ts
withEngineVersion(engineVersion)
```

"EngineVersion specifies the template engine version\nthat should be used to compile/execute the\ntemplate specified in .data and .templateFrom[]."

### fn spec.template.withMergePolicy

```ts
withMergePolicy(mergePolicy)
```



### fn spec.template.withTemplateFrom

```ts
withTemplateFrom(templateFrom)
```



### fn spec.template.withTemplateFromMixin

```ts
withTemplateFromMixin(templateFrom)
```



**Note:** This function appends passed data to existing values

### fn spec.template.withType

```ts
withType(type)
```



## obj spec.template.metadata

"ExternalSecretTemplateMetadata defines metadata fields for the Secret blueprint."

### fn spec.template.metadata.withAnnotations

```ts
withAnnotations(annotations)
```



### fn spec.template.metadata.withAnnotationsMixin

```ts
withAnnotationsMixin(annotations)
```



**Note:** This function appends passed data to existing values

### fn spec.template.metadata.withLabels

```ts
withLabels(labels)
```



### fn spec.template.metadata.withLabelsMixin

```ts
withLabelsMixin(labels)
```



**Note:** This function appends passed data to existing values

## obj spec.template.templateFrom



### fn spec.template.templateFrom.withLiteral

```ts
withLiteral(literal)
```



### fn spec.template.templateFrom.withTarget

```ts
withTarget(target)
```



## obj spec.template.templateFrom.configMap



### fn spec.template.templateFrom.configMap.withItems

```ts
withItems(items)
```

"A list of keys in the ConfigMap/Secret to use as templates for Secret data"

### fn spec.template.templateFrom.configMap.withItemsMixin

```ts
withItemsMixin(items)
```

"A list of keys in the ConfigMap/Secret to use as templates for Secret data"

**Note:** This function appends passed data to existing values

### fn spec.template.templateFrom.configMap.withName

```ts
withName(name)
```

"The name of the ConfigMap/Secret resource"

## obj spec.template.templateFrom.configMap.items

"A list of keys in the ConfigMap/Secret to use as templates for Secret data"

### fn spec.template.templateFrom.configMap.items.withKey

```ts
withKey(key)
```

"A key in the ConfigMap/Secret"

### fn spec.template.templateFrom.configMap.items.withTemplateAs

```ts
withTemplateAs(templateAs)
```



## obj spec.template.templateFrom.secret



### fn spec.template.templateFrom.secret.withItems

```ts
withItems(items)
```

"A list of keys in the ConfigMap/Secret to use as templates for Secret data"

### fn spec.template.templateFrom.secret.withItemsMixin

```ts
withItemsMixin(items)
```

"A list of keys in the ConfigMap/Secret to use as templates for Secret data"

**Note:** This function appends passed data to existing values

### fn spec.template.templateFrom.secret.withName

```ts
withName(name)
```

"The name of the ConfigMap/Secret resource"

## obj spec.template.templateFrom.secret.items

"A list of keys in the ConfigMap/Secret to use as templates for Secret data"

### fn spec.template.templateFrom.secret.items.withKey

```ts
withKey(key)
```

"A key in the ConfigMap/Secret"

### fn spec.template.templateFrom.secret.items.withTemplateAs

```ts
withTemplateAs(templateAs)
```

