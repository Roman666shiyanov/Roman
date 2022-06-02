# Roman
itk uhtrf xtht hre
# авторизация 
и тут пример примерный код
# авторизация 
и тут примерный код
class DB
    {
        MySqlConnection connect = new MySqlConnection("server=localhost;port=3306;username=root;password=;database=data_dictionary;");
        public void openConnection()
        {
            if (connect.State == System.Data.ConnectionState.Closed)
                connect.Open();
        }
        public void closeConnection()
        {
            if (connect.State == System.Data.ConnectionState.Open)
                connect.Close();
        }
        public MySqlConnection getConnection()
        {
            return connect;
        }
