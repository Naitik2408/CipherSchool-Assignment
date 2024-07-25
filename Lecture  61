package graphs;
import java.util.*;
public class GraphAlgos{
    static void dijkstras(int adjMatrix[][],int source){
        int v = adjMatrix.length;
        boolean visited[] = new boolean[v];
        int distance [] = new int[v];
        for(int i=0;i<v;i++){
            distance[i] = Integer.MAX_VALUE;

        }
        distance[source]=0;
        for(int i=0;i<v-1;i++){
            int minVertex = findMinVertex(distance,visited);
            visited[minVertex] =true;
            ///travers neighbours that are unvisited
            for(int j=0;j<v;j++){
                if(adjMatrix[minVertex][j]!=0&&!visited[j]){//not zero means neighbours
                   int newDistance = distance[minVertex]+adjMatrix[minVertex][j];
                    if (newDistance = distance[minVertex] + adjMatrix[minVertex][j];
                    if(newDistance<distance){
                        distance[j] = newDistance;
                    }
                }
            }
        }
        System.out.println("shorted paths from "+source+"are:");
        for(int i=0;i<distance.length;i++){
            System.out.println(distance[i]+" ");
            
        }
        System.out.println();
    }
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        System.out.println("enter number of vertices");
        int v = sc.nextInt();
        System.out.println("enter number of edges");
        int e = sc.nextInt();
        int adjMatrix[][] = new intp[v][v];
        System.out.println("enter all edges : ");
        for(int i=0;i<e;i++){
            int v1 = sc.nextInt();
            int v2 = sc.nextInt();
            int w = sc.nextInt();
            adjMatrix[v1][v2] = w;
            adjMatrix[v2][v1] = w;

        }
        dijkstras(adjMatrix,0);
    }
}
