# Response-Class

using System;
using System.Collections.Generic;
using System.Text;

namespace Entities.Models
{
   public class Response
    {
            public Response()
            {
            }

            public Response(string message, object data)
            {
                this.message = message;
                this.data = data;
            }

            public int code = 200;
            public string status = "Ok";
            public string message = "Successful";
            public object data = new { };
        }

        public class ResponseAccepted
        {
            public ResponseAccepted()
            {
            }

            public ResponseAccepted(string message, object data)
            {
                this.message = message;
                this.data = data;
            }

            public int code = 202;
            public string status = "Accepted";
            public string message = "Successful";
            public object data = new { };
        }

        public class ResponseException
        {
            public ResponseException()
            {
            }

            public ResponseException(string message)
            {
                this.message = message;
            }

            public int code = 500;
            public string status = "Internal Server Error";
            public string message = "Internal Server Error";
        }

        public class ResponseSqlException
        {
            public ResponseSqlException()
            {
            }

            public ResponseSqlException(string message)
            {
                this.message = message;
            }

            public int code = 500;
            public string status = "Data Server Error";
            public string message = "Data Server Error";
        }

        public class ResponseNotFound
        {
            public ResponseNotFound()
            {
            }

            public ResponseNotFound(string message)
            {
                this.message = message;
            }

            public int code = 404;
            public string status = "Resource Not Found";
            public string message = "Resource Not Found";
        }

        public class ResponseUnprocessableEntity
        {
            public ResponseUnprocessableEntity()
            {
            }

            public ResponseUnprocessableEntity(string message)
            {
                this.message = message;
            }

            public int code = 422;
            public string status = "Unprocessable Entity";
            public string message = "Unprocessable Entity";
        }

        public class ResponseUnauthorizeAccess
        {
            public ResponseUnauthorizeAccess()
            {
            }

            public ResponseUnauthorizeAccess(string message)
            {
                this.message = message;
            }

            public int code = 401;
            public string status = "Unauthorize";
            public string message = "Invalide Token! You are not authorize";
        }
    }

