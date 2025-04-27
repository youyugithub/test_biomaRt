# test_biomaRt

```
library(biomaRt)
ensembl <- useMart("ENSEMBL_MART_SNP", dataset = "hsapiens_snp")
rsid <- 'rs12345'
result<-getBM(
  attributes=c('refsnp_id','chr_name','chrom_start'),
  filters="snp_filter",
  values=rsid,
  mart=ensembl)
```
