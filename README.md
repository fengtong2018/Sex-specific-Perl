# Sex-specific-Perl
Rapid identification of sex-specific DNA fragments in Acipenseridae using comparative genomics with high-throughput sequencing


   depth_filtrate.pl
   
      perl depth_filtrate.pl mF.file.list 2 20 > outfile
   
      #mF.file.list is the ctg name from soapdenovo list file, only ctg name.
      
      #2 means calculate site.
      
      #20 means 20 sample`s depth have to > 0.
     
     
   fq2.pl
   
      perl fq2.pl *1.fq *2.fq
   
      #*fq is the fq result from kmer.reads.fq.pl for each smple.
      
      
   kmer_reads_fq.pl
   
      perl kmer.reads.use.pl fq_file.list
   
      #fq_file.list is the fq file`s path.
      
      
   split_depth.pl
   
      perl split_depth.pl depth.file
   
      #the result must output in same folder named with sample name.
      
      
   split_kmer.pl
   
      perl split_kmer.pl all.list 
   
      #all.list is the output file from filterX.
      
      
   sum_depth.pl
   
      perl sum_depth.pl mF.list file.list
   
      #mF.list is the contig name from soapdenovo list file, including > and the number postfix.
      
      #file.list is the folder name from split_depth.pl.
     
