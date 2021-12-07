# nats-javakv-101
Basic kick the tires on NATS Key-Value API (Java)

# API Notes

```text
KeyValueManagement kvm = nc.keyValueManagement();
KeyValue kv = nc.keyValue(BUCKET_NAME);
```
| Type | Methods |
| --- | --- |
| KeyValueManagement | createBucket(), deleteBucket(), getBucketInfo(), purgeBucket(), purgeKey(), getHistory(), keys(), bucketNames() |
| BucketConfiguration | getBackingConfig(), getName(), getMaxValues(), getMaxHistoryPerKey(), getMaxBucketSize(), getMaxValueBytes(), getTtl(), getStorageType(), getDuplicateWindow(), toString(), builder() |
| BucketInfo |getConfiguration(), getRecordCount(), getByteCount(), getLastSequence(), getCreateTime(), toString() |
| KeyValue | put (string, byte array, long), getValue(), getStringValue(), getLongValue(), delete, getEntry() |
| KvEntry | getBucket(), getKey(), getSeq(), getData(), getCreated(), getKvOperation(), toString() |

Note: No Watch?
