# idea
Demo1
class SortReady{
    public static boolean less(Comparable a,Comparable b){
        return  a.comparaTo(b);
    }

    public static void exch(Comparable[] a,int index1,int index2){
        if(a.length==0) return;
        Compara tmp=a[index1];
        a[index1]=a[index2];
        a[index2]=tmp;
    } 
}


class Merge{
    private Comparable []axc;
    public static void sort(Comparable []a){
       axc=new Comparable[a.length];
       sort(a,0,a.length-1);
    }
    
    public static void sort(Comparable []a,int lo,int hi){
        if(hi<=lo) return;
        int mid=lo+(hi-lo)/2;
        sort(a,lo,mid);
        sort(a,mid+1,hi);
        merage(a,lo,mid,hi);
    }
    
    public static void merge(Comparable[] a,int lo,int mid,int hi){
        int i=lo;
        int j=mid+1;
        for(int k=lo;k<hi;k++){
          axc[k]=a[k];
        }
        for(int k=lo;k<hi;k++){
          if(i>mid)                         a[k]=axc[j++];
          else if(j>hi)                     a[k]=axc[i++];
          else if(less(axc[j],axc[i]))      a[k]=axc[j++];
          else                              a[k]=axc[i++];
        }
    }  
}


class MergeBu{
     private Comparable[] axc2;
     public static void sort(Comparable []a,int lo,int hi){
          axc2=new Comparable[a.length];
          for(int i=1;i<sz;i=sz+sz)
     
     
     
     }







}
