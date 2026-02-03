1. Once the data is ingestion ready from source to raw, we should always make sure the below.
    1. If the data is ingested to RAW, will it be idempotent - if we perform same action again and again like re-running jobs, there should be no duplicates created. The data should not be altered.
    2. Once the data enters RAW, it should be durable - even if there is system crash or pipeline failure or anything, data that is already in RAW should exist.
    3. Auditability - This is mainly for tracebility of what data entered RAW, when, where etc. This is why we give ingest with additional details such as metadata.
    4. Immutablity - RAW is append only. Data should not change or overright. Once a data \ enters raw, it will be kept as it is, there is a change, it will be versioned based on hash. (No updates or no deletes)
    