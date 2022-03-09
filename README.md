# Lab7_info-tech
lab 7 for info tech in c#

 class Program
    {
        static void Main(string[] args)
        {
            double usrMoney;
            
            usrMoney = GetTheUserMoney();

        }
        public static double GetTheUserMoney()
        {
            double money;
            bool tryParse;
            Console.WriteLine("Please input the amount of money you have? ");

            tryParse = double.TryParse( Console.ReadLine() ,out money);

            while (!tryParse)
            {
                Console.WriteLine("What youve just imported isn't ");
            }


            return money;
        }
    }
}
