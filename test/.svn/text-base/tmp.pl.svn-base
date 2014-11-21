open IN, "evidence.db-";

while($line = <IN>){
	chomp($line);
	if($line =~ /\!category/){
		next;
	}
	$a = 0;
	while($line =~ /Paper([0-9]*)/g){
		if($1 > 1000){
			$a = 1;
			break;
		}
	}
	if($a == 1){
		next;
	}else{
		print "$line\n";
	}


}
