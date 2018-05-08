class Program
{
 
 
 static void Main(string[] args)
 {
            String s = "asdasdé, aasdadasdaá, saduasudnus é";

            Regex reg = new Regex("[éáíóú']");
            Match m = reg.Match(s);
            while (m.Success)
            {
                String replacement = "\\u" + ((int)m.Value[0]).ToString("X4");
                s = s.Replace(m.Value, replacement);
                m = m.NextMatch();
            }
            Console.WriteLine(s);
  }
         
}
