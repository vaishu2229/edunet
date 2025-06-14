import java.util.*;
class Unwtadj{
    int vertices;
    LinkedList<LinkedList<Integer>> adjList;
    Unwtadj(int n){
        vertices=n;
        adjList=new LinkedList<>();
        for(int i=0;i<vertices;i++){
            adjList.add(new LinkedList<>());
        }
    }
    void addEdge(int src,int dest){
        adjList.get(src).add(dest);
        adjList.get(dest).add(src);
    }
    void removeEdge(int src,int dest){
        adjList.get(src).remove(Integer.valueOf(dest));
        adjList.get(dest).remove(Integer.valueOf(src));
    }
}
public class Main
{
public static void main(String[] args) {
System.out.println("Hello World");
}
}
