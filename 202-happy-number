class Solution {
public:
    bool isHappy(int n) {
		int sum=0;
		unordered_set<int> cycle;
		cycle.insert(n);
		while(n!=1){
			while(n){
				sum+=(n%10)*(n%10);
				n=n/10;
			}
			if(cycle.find(sum)==cycle.end())
		    cycle.insert(sum);
			else return 0;
			n=sum;
			sum=0;
		}
		return  1;
    }
};
